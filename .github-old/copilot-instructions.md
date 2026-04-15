---
source-git-commit: f6a305c6a4e700525b570bbe280e5d1049d06537
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---
## Función

Ayude a los asistentes de codificación de IA a realizar ediciones pequeñas y seguras en el repositorio de documentación de GenStudio for Performance Marketing.

## Arquitectura de alto nivel (breve)
- Este repositorio es un sitio de documentación compuesto por Markdown en `help/` con inclusiones compartidas en `help/_includes/` e imágenes revisadas en `help/_includes/assets/`.
- Las notas de la versión, la guía del usuario y el contenido de extensibilidad están en directo en `help/`. Los cambios grandes en el contenido deben conservar el contenido principal y la estructura de encabezados existente.
- El sitio se crea con Jekyll y se aloja en páginas de GitHub. El proceso de compilación utiliza convenciones estándar de Jekyll con algunos complementos personalizados.

## Convenciones específicas del proyecto
- Reglas de cursor: la automatización y la guía personalizadas se aplican en `.cursor/rules/*.mdc`. Ejemplos: `.cursor/rules/docs-lint.mdc` (proceso de pelusa), `.cursor/rules/generate-release-notes.mdc` (señala a la aptitud de las notas de la versión al editar `help/user-guide/release-notes.md`). Siga estos pasos para tareas automatizadas.
- Aptitudes de agente: los flujos de trabajo de tareas están activos en `.cursor/skills/<name>/SKILL.md`. Ejemplo: `.cursor/skills/generate-release-notes/SKILL.md` (procedimiento completo de notas de la versión de GenStudio; usar con `examples.md` y `reference.md` en la misma carpeta).
- Nombres de archivo y frontmatter:
   - Notas de la versión: conserve el frontmatter de Experience League existente en `help/user-guide/release-notes.md` (consulte `.cursor/skills/generate-release-notes/reference.md#frontmatter`); la regla fina `.cursor/rules/generate-release-notes.mdc` se adjunta automáticamente cuando se edita ese archivo.
   - Utilice kebab-case para los archivos de reglas y la extensión `.mdc`.
- Convenciones de formato: Los documentos utilizan Markdown al estilo de GitHub. Los encabezados generalmente siguen las mayúsculas y minúsculas de las oraciones y los párrafos cortos. Prefiera `*` viñetas para las listas de las notas de la versión y `###` para las secciones de características.

## Directrices de estilo de documentación
- Siga la [Guía de estilo de escritura de Microsoft](https://learn.microsoft.com/en-us/style-guide/) para ver las prácticas recomendadas de documentación técnica:
   - Escriba frases claras y concisas centradas en las acciones del usuario
   - Usar la voz activa y el tiempo presente
   - Dividir texto en fragmentos cortos analizables
   - Mantenga un tono cálido y directo mientras mantiene la precisión técnica
- Creación de Markdown:
   - Utilice mayúsculas y minúsculas en los encabezados (escriba mayúsculas en la primera palabra solamente)
   - Utilice párrafos cortos (2-3 frases) para facilitar la lectura
   - Agregar líneas en blanco antes y después de encabezados y listas
   - Utilice comillas invertidas para los elementos de la interfaz de usuario, las rutas de archivo y el código
   - Incluir texto alternativo para todas las imágenes
   - Vínculo a secciones específicas mediante un texto descriptivo

## Reglas de seguridad para las ediciones (qué debe hacer la IA)
- Nunca agregue ID de Jira, vínculos internos o referencias solo corporativas a documentos públicos. Ver `.cursor/skills/generate-release-notes/SKILL.md` (sección **Contenido prohibido**).
- Conservar YAML de frontmatter exactamente al editar archivos que lo incluyen. Muchas plantillas y notas de la versión dependen de claves fijas (título, descripción, función, exl-id).
- Para las correcciones de pelusa, prefiera las ediciones automatizadas e idempotentes de `.cursor/rules/docs-lint.mdc` (quite los espacios finales, asegúrese de que la nueva línea sea final). Comandos de ejemplo utilizados por humanos:

```sh
sed -i '' 's/ $//' <file>
sed -i '' '$ { /^$/d; }' <file> && echo "" >> <file>
```

## Ejemplos (qué cambiar y cómo)
- Correcciones de copias pequeñas: actualice el texto dentro de `help/` archivos Markdown, mantenga intactos los encabezados y anclajes.
- Actualizaciones de imágenes: haga referencia a imágenes en `help/_includes/assets/`. No mueva ni cambie el nombre de las imágenes sin actualizar todas las referencias.

## Dónde buscar primero
- `help/_includes/` — fragmentos e imágenes compartidos.
- `.cursor/rules/`: instrucciones de automatización y vinculación; utilícelas como reglas autoritativas para el formato y los procesos.
- `markdownlint_custom.json`: invalidaciones de markdownlint locales.
- `.github/pull_request_template.md` — Expectativas de PR.

## Cuándo preguntar al humano
- Si un cambio requiere la ejecución o modificación de herramientas basadas en Docker (la regla de lint menciona Docker) o afecta a las canalizaciones de compilación del sitio.
- Si un archivo hace referencia a una configuración externa desconocida (por ejemplo, falta `markdownlint.json`), pregunte si desea crear o omitir.

## Comandos mínimos para humanos

```sh
# Install linter (if not present)
npm install -g markdownlint-cli

# Run lint locally using project config
markdownlint --config markdownlint_custom.json "help/**/*.md"

# Project lint via yarn (preferred if available in environment)
yarn lint
```

---
Si lo desea, puedo combinarlo en `.github/copilot-instructions.md` en el repositorio (o ajustar la redacción/longitud). ¿Qué debo cambiar o agregar?
