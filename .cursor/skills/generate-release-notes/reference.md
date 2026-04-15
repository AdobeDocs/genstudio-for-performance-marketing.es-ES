---
source-git-commit: f6a305c6a4e700525b570bbe280e5d1049d06537
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 6%

---
# Referencia: creación de notas de la versión

## Frontmatter

La página activa [help/user-guide/release-notes.md](../../help/user-guide/release-notes.md) incluye metadatos de Experience League que van más allá de un conjunto mínimo (por ejemplo, `TQID`, `product_v2`, `feature_v2`, ID de taxonomía).

**Reglas:**

- Al editar el contenido de la nota de versión **body**, **conserve las claves y los valores de la frontmatter** existentes a menos que la tarea pida explícitamente que se cambien los metadatos.
- No elimine los metadatos de taxonomía o producto para que coincidan con una plantilla más corta.
- Los conceptos requeridos para las páginas ExL generalmente incluyen `title`, `description` y `role`; siga la [guía de metadatos de Experience League](https://experienceleague.adobe.com/en/docs/authoring-guide/using/authoring/using-metadata) para las páginas nuevas.

## Fuentes internas (KT y wikis de versiones)

Utilice estos campos **solo mientras redacta**; las notas de la versión publicadas no deben hacer referencia a documentos internos.

### Documentos de transferencia de conocimientos (KT)

Extraer de:

| Campo | Utilice |
|-------|-----|
| Descripción | Explicación de las funciones principales |
| Argumento del ascensor | Propuesta de valor |
| Funciones entregadas | Comportamiento concreto |
| Declaración de problema | Punto problemático del usuario |
| Tipo y fecha de versión | Intervalo |

### Liberar páginas wiki

Agrupar y ámbito por:

| Campo | Utilice |
|-------|-----|
| Fecha de lanzamiento (versión fija) | Misma fecha → mismo lote de notas de la versión |
| Iniciativa | Solo contexto; no vincular internamente en texto público |
| PM presenta la función utilizando KT | Puede haber señales con detalles de KT más profundos |

**Regla de ámbito:** Los elementos que comparten la misma fecha de lanzamiento (versión de corrección) pertenecen al mismo bloque de lanzamiento mensual.

## Vinculación de documentación

- Vincular a la frase **más relevante** (por ejemplo, vincular &quot;recursos de imagen y vídeo no compatibles&quot; a la sección de formatos de anuncio).
- Preferir `#anchor` vínculos en la subsección derecha.
- Las páginas de información general son aceptables cuando no existe ningún anclaje más profundo.

## Rutas de documentación comunes

| Área | Prefijo de ruta |
|------|-------------|
| Crear | `/help/user-guide/create/` |
| Contenido | `/help/user-guide/content/` |
| Activación | `/help/user-guide/activation/` |
| Aprobaciones | `/help/user-guide/approvals/` |
| Perspectivas | `/help/user-guide/insights/` |
| Directrices | `/help/user-guide/guidelines/` |
| Plantillas | `/help/user-guide/templates/` |
| Campañas | `/help/user-guide/campaigns/` |
| Extensibilidad | `/help/extensibility/` |
