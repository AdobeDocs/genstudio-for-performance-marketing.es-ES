---
name: polish-release-notes
description: ""
notes: refines only newly added
source-git-commit: 1a33b08048233c5f9a82b5f428082aa5c71b0052
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---


# Notas de la versión de GenStudio en polaco

**Archivo de destino canónico:** [help/user-guide/release-notes.md](../../../help/user-guide/release-notes.md)

**Ejemplos:** [samples.md](examples.md)

**Flujo de trabajo de borrador (flujo ascendente):** [generate-release-notes](../generate-release-notes/SKILL.md)

## Ámbito (obligatorio)

**Solo** contenido polaco que el usuario identifica como **recién agregado** en esta ronda:

- **En el archivo:** `###` subsecciones bajo el único encabezado `## YYYY.MM {#latest}` en `help/user-guide/release-notes.md`.
- **No** edite el título de página, el párrafo de introducción, el frontmatter ni ningún texto debajo de **Notas de la versión anteriores** (bloques contraíbles de `+++`).
- **No** edite `##` bloques mensuales anteriores o `###` preexistentes en la misma sección `{#latest}` a menos que el usuario **se lo pida explícitamente**.
- Si no está claro qué `###` son nuevos, **pregunte** o use **git diff** / edite el contexto antes de cambiar la prosa.
- **Contenido pegado:** solo marca de pulido que el usuario pega cuando confirma que coincide con esas **mismas** subsecciones nuevas (no trate la pegada no relacionada como dentro del ámbito).

Mantener diferencias **mínimas**: solo saltos de párrafo y redacción, sin refactores de activación en ninguna otra parte del archivo.

## Voz y tono

- Escriba como **redactor** para las notas de la versión del producto: **conciso**, **analizable** y **energizado** acerca de **nuevo valor**; obtenga resultados y aprenda &quot;lo que necesita&quot;; use verbos fuertes y lenguaje claro de beneficios.
- **Manténgase al pendiente:** no hay afirmaciones que vayan más allá de lo que ofrece la función; combine el tono Experience League/Adobe (seguro y claro, no sensacionalista).
- **Genera emoción** con **beneficios específicos** y deltas (lo que los especialistas en marketing pueden hacer ahora, qué fricción se elimina), no exageraciones vacías ni superlativos sin fundamento.

## Reglas de párrafo

- Cada párrafo: **2-3 frases**. **Nunca más de tres frases** en un párrafo: si necesitas más, comienza un **nuevo párrafo**.
- Opcional: si un párrafo aún se ejecuta más de **~3 líneas** en documentos procesados con una longitud de línea típica, divida más.

## No añadir

- **Contenido de procedimientos &quot;**&quot;: pasos numerados, &quot;haga clic en **[!UICONTROL ...]** y luego...&quot;, tutoriales completos de la interfaz de usuario o frases de tutoriales. Las notas de la versión resumen **lo que se envió** y **por qué importa**, no lecciones prácticas.
- Contenido que viola [Contenido prohibido](../generate-release-notes/SKILL.md#prohibited-content) en la aptitud generada (sin claves Jira, URL solo internas, wiki como prueba, etc.).

## Conservar (no eliminar ni reescribir estructuralmente)

- `[!DNL …]`, `[!UICONTROL …]`, `[!BADGE …]` y otros códigos abreviados de ExL.
- Vínculos de documentación y patrones de anclaje **relativos** existentes: `[phrase](/help/...)` en texto de anclaje significativo.
- Los bloques de distintivo de Beta son exactamente los mismos que se usan en [generate-release-notes example](../generate-release-notes/examples.md).

## Lista de comprobación de flujo

1. [ ] Confirmar **qué** `###` bajo `## … {#latest}` están en el ámbito (nuevo en esta ronda).
2. [ ] Para cada `###` en el ámbito, ajuste la copia según [voz y tono](#voice-and-tone) y [reglas de párrafo](#paragraph-rules).
3. [ ] Eliminar o acortar cualquier instrucción de **procedimientos**; conservar **resultados de usuario**.
4. [ ] Verifique que los vínculos y los códigos abreviados sigan siendo válidos; realice un análisis rápido de los identificadores internos o los patrones prohibidos según [comprobaciones de calidad](#quality-checks).

## Comprobaciones de calidad

- [ ] Solo cambiaron los **nuevos** `###` bloques acordados menores de `{#latest}`; no se tocaron los archivos ni los meses anteriores.
- [ ] No hay ID nuevos de estilo Jira, URL de wiki internas ni idioma de &quot;ver ticket&quot;.
- [ ] párrafos son **2-3 frases** cada una (máximo tres frases por párrafo).
- [ ] La copia permanece **objetiva** y alineada con la capacidad descrita.

## Recursos adicionales

- [samples.md](examples.md) — patrones antes/después.
- [generate-release-notes](../generate-release-notes/SKILL.md): redacción, archivado, distintivos de Beta y vinculación.
