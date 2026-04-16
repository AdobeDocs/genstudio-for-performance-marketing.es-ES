---
name: polish-release-notes
description: ""
notes: refines only newly added
source-git-commit: ee2875f35035e23e2577adbde5f408702b77d233
workflow-type: tm+mt
source-wordcount: '630'
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

## Eliminar durante el pulido (programación de versiones)

Drafts sometimes include **italicized** lines (`_…_` or `*…*`) about **availability**—for example limited release, Summit timing, GA, broader rollout, or Beta **windows**. That language belongs in **release management**, not in polished customer-facing notes for this page.

- **Remove entirely** those **italic** lines or **trailing italic clauses** when their **primary purpose** is scheduling or rollout status (including **GA**, **limited release**, **Summit**, or similar).
- **Do not** strip ordinary (non-italic) sentences that describe product behavior—only scheduling copy that was set in **italics** as a disclaimer.
- **Keep** the **[!BADGE Beta]** block when the feature is Beta; the badge is the supported pattern for Beta, not a separate italic scheduling line.
- After removal, **tighten surrounding prose** if a paragraph now starts or ends awkwardly; do not replace removed italics with new scheduling sentences unless the user explicitly asks.

## Preserve (do not strip or rewrite structurally)

- `[!DNL …]`, `[!UICONTROL …]`, `[!BADGE …]`, and other ExL shortcodes.
- Existing **relative** documentation links and anchor patterns: `[phrase](/help/...)` on meaningful anchor text.
- Beta badge blocks exactly as used in [generate-release-notes examples](../generate-release-notes/examples.md).

## Workflow checklist

1. [ ] Confirm **which** `###` under `## … {#latest}` are in scope (new this round).
2. [ ] For each in-scope `###`, tighten copy per [Voice and tone](#voice-and-tone) and [Paragraph rules](#paragraph-rules).
3. [ ] Remove or shorten any **how-to** instructions; keep **user outcomes**.
4. [ ] Strip **italic (or italic-styled) scheduling and availability** lines per [Remove during polish (release scheduling)](#remove-during-polish-release-scheduling).
5. [ ] Verify links and shortcodes still valid; run a quick scan for internal IDs or banned patterns per [Quality checks](#quality-checks).

## Quality checks

- [ ] Only the agreed **new** `###` blocks under `{#latest}` changed; archives and older months untouched.
- [ ] No new Jira-style IDs, internal wiki URLs, or “see ticket” language.
- [ ] No **scheduling-only** italic disclaimers (GA, limited release, Summit rollout, etc.) remain in polished `{#latest}` subsections—those were removed per [Remove during polish (release scheduling)](#remove-during-polish-release-scheduling); Beta badge blocks are fine where applicable.
- [ ] Paragraphs are **2–3 sentences** each (max three sentences per paragraph).
- [ ] Copy stays **factual** and aligned with the described capability.

## Recursos adicionales

- [examples.md](examples.md) — before/after patterns.
- [generate-release-notes](../generate-release-notes/SKILL.md) — drafting, archival, Beta badges, linking.
