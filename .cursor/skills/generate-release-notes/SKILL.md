---
name: generate-release-notes
description: ""
source-git-commit: 1a33b08048233c5f9a82b5f428082aa5c71b0052
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---


# Generar notas de la versión de GenStudio

**Archivo de destino canónico:** [help/user-guide/release-notes.md](help/user-guide/release-notes.md)

**Ejemplos completos:** [samples.md](examples.md)

**Asignación de campos KT/wiki y rutas de documentos:** [reference.md](reference.md)

## Lista de comprobación de flujo

Trabaje en este orden. Copie la lista de comprobación y rastree el progreso de las ediciones de varios pasos.

1. [ ] Abra `help/user-guide/release-notes.md` y lea el bloque `## YYYY.MM {#latest}` actual y el área **Notas de la versión anteriores**.
2. [ ] Si se agrega una **nueva** versión mensual: archive la última versión actual (consulte [Archivar la última versión anterior](#archive-previous-latest)).
3. [ ] Agregue o edite la sección `## YYYY.MM {#latest}` principal (el mes más reciente en la parte superior de la lista de versiones).
4. [ ] Para cada elemento, aplique [reglas de decisión](#decision-rules) (característica `###` frente a **correcciones y mejoras**, distintivo de Beta o no).
5. [ ] Agregar o comprobar vínculos de documentación en la frase más relevante (consulte [reference.md](reference.md#documentation-linking)).
6. [ ] Ejecute [comprobaciones de calidad](#quality-checks) antes de finalizar.
7. [ ] Conservar [frontmatter](reference.md#frontmatter) en la página a menos que la tarea actualice explícitamente los metadatos.

## Reglas de decisión

Utilice estas reglas &quot;if/then&quot; para que el contenido aterrice en el lugar correcto:

| Si | Entonces |
|----|------|
| La funcionalidad es nueva y está en Beta | Agregue la línea del distintivo de Beta inmediatamente debajo del encabezado `###` (vea [samples.md](examples.md)). |
| El material de Source etiqueta explícitamente el elemento como **corrección** o **mejora** | Ponlo bajo `### Fixes and enhancements` con `*` viñetas solamente. |
| El elemento es una nueva historia de funcionalidad o característica | Use una sección de características `###` con de 1 a 3 frases (no la lista de correcciones). |
| No está seguro de si algo es una corrección o una función | De forma predeterminada, se usa una sección de características `###` a menos que el origen indique claramente una corrección o mejora. |

**Regla de sección de correcciones:** No agregue viñetas a **Correcciones y mejoras** a menos que el origen esté etiquetado explícitamente como una corrección o mejora.

## Archivar más reciente anterior

Al presentar un nuevo(a) `## YYYY.MM {#latest}`:

1. Corte toda la sección `## YYYY.MM {#latest}` anterior (desde su encabezado hasta el final del contenido de esa versión, antes de las `##` o **notas de versiones anteriores** siguientes).
2. Péguelo en **notas de versiones anteriores**, dentro de un bloque contraíble.
3. Reemplazar el encabezado antiguo por: `+++Notes from YYYY.MM.DD+++` (usar la fecha de lanzamiento real; dar formato como en las notas existentes en el archivo).
4. Elimine `{#latest}` del encabezado archivado; la nueva sección superior es la única con `{#latest}`.
5. Mantenga el orden cronológico dentro de **Notas de la versión anteriores** (los bloques archivados más recientes hacia la parte superior a menos que el archivo ya utilice un orden diferente—**coincide con el archivo existente**).

## Estructura requerida

### Título e introducción de la página

Después del front-matter, utilice:

```markdown
# GenStudio for Performance Marketing release notes

This release information details the latest updates to the GenStudio for Performance Marketing application.
```

Si el archivo ya utiliza una frase de introducción ligeramente diferente (por ejemplo, &quot;proporciona&quot; en lugar de &quot;detalles&quot;), mantenga la coherencia con el resto de la página.

### Encabezado de la última versión

- Formato: `## YYYY.MM {#latest}` para el bloque de versión más reciente.
- Solo hay un anclaje `{#latest}` en la página.

### Secciones de funciones

- Usar `###` para las categorías de características principales.
- Presente el tiempo, 1-3 oraciones, aclarar qué/por qué y las acciones del usuario cuando sea útil.
- Nombres de productos: `[!DNL Create]`, `[!DNL Content]`, `[!DNL Insights]`, etc.
- Interfaz de usuario: `[!UICONTROL Control Name]` donde corresponda.
- Énfasis: `_italics_` para áreas o secciones de la interfaz de usuario; `**bold**` para términos clave con moderación.

### distintivo de Beta

Usar exactamente:

```markdown
[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}
```

### Vínculos de documentación

- Patrón: `[link text](/help/user-guide/section/page.md#anchor)`
- Prefiera los anclajes; vincule la frase que a los usuarios les importa, no &quot;haga clic aquí&quot;.

### Correcciones y mejoras

- Las líneas de viñetas utilizan `*`.
- Solo los elementos etiquetados explícitamente como corrección/mejora en el material de origen.
- Mismas convenciones terminológicas y de vínculos que las funciones.

## Contenido prohibido

- **no** incluye claves Jira, números de problemas internos, URL de solo uso interno o enlaces de wiki corporativos en las notas de la versión publicadas.
- **no** cita documentos, tickets o herramientas internas de transferencia de conocimientos como prueba; solo resume los resultados de cara al usuario.
- **no** duplica `{#latest}` en múltiples secciones.

## Comprobaciones de calidad

Antes de completar la tarea:

- [ ] Todos los vínculos relativos nuevos o cambiados se resuelven en rutas reales bajo `help/` siempre que sea posible.
- [ ] características de Beta incluyen el fragmento de distintivo de Beta donde sea necesario.
- [ ] La terminología coincide con las notas de la versión existentes (`[!DNL …]`, `[!UICONTROL …]`).
- [ ] Analiza el borrador en busca de ID internos accidentales (`[A-Z]+-\d+`), URL de wiki o el idioma &quot;ver Jira&quot;; elimínalos.
- [ ] **Correcciones y mejoras** solo contiene correcciones o mejoras etiquetadas explícitamente.
- [ ] La sección anterior más reciente se archivó correctamente cuando se agregó un nuevo mes.

## Fuentes de contenido (resumen)

Al extraer de los documentos de transferencia de conocimientos o de las wikis de versiones internamente, asigne los campos tal como se describe en [reference.md](reference.md#internal-sources-kt-and-release-wikis). La página enviada debe leerse como documentación de usuario independiente.

## Opcional: pulir nuevas subsecciones

Después de agregar contenido nuevo de `###` en `{#latest}`, ejecute [notas de la versión en polaco](../polish-release-notes/SKILL.md) para un pase con estilo de editor de copias (tono de avance de beneficios, **2-3 oraciones por párrafo**, sin procedimientos) **solo** en esas **nuevas** subsecciones—**no** en notas de versiones anteriores o texto preexistente a menos que se solicite explícitamente.

## Recursos adicionales

- [samples.md](examples.md): ejemplos listos para pegar (características, correcciones, bloque de archivo).
- [reference.md](reference.md): notas de frontmatter, rutas de documentos y estrategia de vinculación.
- [Notas de la versión en polaco](../polish-release-notes/SKILL.md) — pase editorial opcional para `###` recién agregado en `{#latest}`.
