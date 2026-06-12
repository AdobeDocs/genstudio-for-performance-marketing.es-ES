---
source-git-commit: c3c6aa86f4f520d020f8928612d1be6be1599652
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 3%

---
# Referencia: consumir fuentes de versión (MCP)

## Ceremonia de descubrimiento de páginas

| Patrón | Ejemplo |
|---------|---------|
| Título | `YYYY/MM Release Ceremony` en el espacio **GenStudio** |
| De Jira | Vínculo wiki en el ticket `description` (preferido) |
| Reserva de CQL | `title ~ "2026/06 Release Ceremony" AND space = GenStudio` |

## Grupos de funciones de ceremonia

Las wikis de la ceremonia de lanzamiento contienen hasta **dos** tablas de características. Analizar ambos desde **almacenamiento** HTML.

### Funciones de la versión de GA

- Encabezado de sección: `GA Release Features` (`<h2>`)
- Subencabezado: `Feature Group:` con vínculo de Floodgate opcional
- Las columnas de la tabla incluyen **Tipo** (`GA`, `Limited`, `EA`, `Beta` o vacío)
- **Columna de documentación de KT**: `<ac:link><ri:page ri:content-title="..."/></ac:link>`

Extracción por fila:

| Campo | Origen |
|-------|--------|
| `featureDescription` | Primer(a) `<td>` en fila de datos |
| `type` | Escribir texto de celda de columna |
| `ktPageTitle` | `ri:content-title` en la columna KT |
| `jiraKeys` | `ac:macro ac:name="jira"` → `key` parámetro (solo interno) |
| `releaseTier` | `ga` cuando Type es `GA`; tipo de herencia para otros valores de GA-table |

### Funciones de la versión de Beta

- Encabezado de sección: `Beta Release Features` (puede ser **ausente** en algunos meses)
- Segunda tabla; **sin columna Type** — cada fila es Beta
- La misma extracción de KT y Jira que la tabla de GA
- Establecer `releaseTier: beta` y `requiresBetaBadge: true` en cada fila de sección de Beta

Si falta la sección Beta, registre cero filas de Beta y continúe.

### Patrones de almacenamiento de HTML

```html
<ac:link><ri:page ri:content-title="Translation on HZ Canvas" /></ac:link>
<ac:structured-macro ac:name="jira" ...><ac:parameter ac:name="key">GS-23218</ac:parameter></ac:structured-macro>
```

## Uso de la herramienta MCP

| Paso | Herramienta | Parámetros |
|------|------|------------|
| Ticket | `jira_getIssue` | `issueKey`, `expand: renderedFields` opcional |
| Ceremonia | `confluence_getContent` | `contentId`, `bodyMode: storage` |
| Búsqueda KT | `confluence_searchContent` | `cql: title = "<KT title>" AND space = GenStudio` |
| Cuerpo KT | `confluence_getContent` | `contentId`, `bodyMode: text`, `maxBodyChars: 50000` |

**No** use `bodyMode: text` para páginas de ceremonia al analizar vínculos KT.

## Asignación de campos KT (entradas de redacción)

Asigne a generate-release-notes; no pegue en notas de versiones públicas literalmente.

| Sección KT | Utilice |
|------------|-----|
| Descripción | Capacidad principal |
| Parcela de ascensor | Propuesta de valor |
| Funciones entregadas | Comportamiento concreto |
| Declaración de problema | Dolor de usuario (solo contexto) |
| Tipo y fecha de versión | GA/Beta/Limited (interna); impulsa la decisión del distintivo |

## Filtros de inclusión

Confirmar ámbito con el usuario cuando no esté claro. Ajustes preestablecidos comunes:

| Preestablecido | Incluye |
|--------|----------|
| `ga_only` | Filas de la tabla de GA donde Tipo = `GA` |
| `ga_and_beta` | **Valor predeterminado recomendado para meses futuros** — Filas de GA donde Tipo = `GA` **más todas** las filas de la tabla Características de la versión de Beta |
| `ga_plus_empty` | Tabla de GA: Tipo = `GA` o Tipo vacío |
| `all_except_pilot` | Filas de tabla de GA excepto `Limited`; más la sección de Beta al usar `ga_and_beta` |
| `all_with_badges` | Todas las filas de la tabla GA; las filas de la sección Beta siempre obtienen el distintivo Beta |

## Entrega de insignias de Beta

| Condición | `requiresBetaBadge` |
|-----------|---------------------|
| Fila de la tabla **Características de la versión de Beta** | `true` |
| Fila de tabla de GA con tipo = `Beta` | `true` |
| Fila de tabla de GA con tipo = `GA` | `false` |

Descendente: [reglas de decisión para generar notas de la versión](../generate-release-notes/SKILL.md#decision-rules) y [fragmento de distintivo de Beta](../generate-release-notes/SKILL.md#beta-badge).

## Carga útil de transferencia (informal)

Pase a generate-release-notes como lista de elementos:

```yaml
- featureDescription: "YouTube Shorts"
  releaseTier: ga
  requiresBetaBadge: false
  ktPageTitle: "YouTube Shorts (Create + Activate)"
  # extracted KT fields: description, elevatorPitch, featuresDelivered, ...
```
