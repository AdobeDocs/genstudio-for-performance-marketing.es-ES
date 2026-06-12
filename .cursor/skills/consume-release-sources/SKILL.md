---
name: consume-release-sources
description: ""
source-git-commit: c3c6aa86f4f520d020f8928612d1be6be1599652
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---


# Consumir fuentes de versión (Jira + MCP de confluencia)

**Borrador descendente:** [generate-release-notes](../generate-release-notes/SKILL.md) → [polish-release-notes](../polish-release-notes/SKILL.md) opcionales

**Referencia de análisis:** [reference.md](reference.md)

**Archivo de salida de destino (solo flujo descendente):** [help/user-guide/release-notes.md](../../help/user-guide/release-notes.md)

## Requisitos previos

- **Jira MCP** (`jira_getIssue`, `jira_searchIssues`) autenticado
- **MCP de confluencia** (`confluence_getContent`, `confluence_searchContent`) autenticado
- Clave de vale Jira del nombre de la rama (`GS-#####`), entrada del usuario o descripción del vale

## Lista de comprobación de flujo

1. [ ] **Resolver ticket Jira** — `jira_getIssue` con `issueKey`. Lea `description` el enlace wiki de la ceremonia y el mes de lanzamiento.
2. [ ] **Localizar página de ceremonia** — usar URL de wiki del ticket; CQL de reserva: `title ~ "YYYY/MM Release Ceremony" AND space = GenStudio`.
3. [ ] **Recuperar cuerpo de ceremonia** — `confluence_getContent` con `bodyMode: storage` (obligatorio; `text` pierde vínculos KT y estructura de tabla).
4. [ ] **Analizar grupos de características** — extraer filas de **Características de la versión de GA** y **Características de la versión de Beta** (véase [reference.md](reference.md#ceremony-feature-groups)).
5. [ ] **Aplicar filtro de inclusión** — por ámbito de usuario (consulte [reference.md](reference.md#inclusion-filters)); confirmar el recuento de filas de Beta (puede ser cero).
6. [ ] **Resolver páginas KT** — `confluence_searchContent` por título KT; `confluence_getContent` con `bodyMode: text`.
7. [ ] **Extraer campos KT** — Descripción, Paso de ascensor, Funciones entregadas, Declaración de problema, Tipo de versión y Fecha.
8. [ ] **Establecer indicadores de Beta** — `requiresBetaBadge: true` para filas de sección de Beta o filas de tabla GA con tipo `Beta`.
9. [ ] **Entrega** a [generate-release-notes](../generate-release-notes/SKILL.md) con lista de filas estructuradas (sin referencias de wiki/Jira en la copia enviada).

## Etiquetado Beta (entrega para generar aptitud)

Cuando `requiresBetaBadge: true`, la sección `###` de la cadena descendente debe incluir inmediatamente debajo del encabezado:

```markdown
[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}
```

No agregue renuncias de programación en cursiva para Beta; el distintivo es el patrón admitido.

## Prohibido en las notas de versión enviadas

Los ID internos, las URL de wiki, las citas de KT y las claves de Jira permanecen solo en esta fase de ingesta. Resumir los resultados de cara al usuario en la página pública por [contenido prohibido generar notas de la versión](../generate-release-notes/SKILL.md#prohibited-content).

## Abandono

Si las llamadas MCP fallan, pídale al usuario que pegue contenido de ceremonia y KT y, a continuación, continúe con generate-release-notes utilizando la asignación de campos KT [reference.md](../generate-release-notes/reference.md#internal-sources-kt-and-release-wikis).

## Recursos adicionales

- [reference.md](reference.md): análisis de ceremonia, CQL, filtros de inclusión, parámetros MCP
- [generate-release-notes](../generate-release-notes/SKILL.md): archivo, borrador, vínculos, comprobaciones de calidad
- [polish-release-notes](../polish-release-notes/SKILL.md) — pase editorial en el nuevo `###` en `{#latest}`
