---
source-git-commit: f6a305c6a4e700525b570bbe280e5d1049d06537
workflow-type: tm+mt
source-wordcount: '80'
ht-degree: 0%

---
# Ejemplos de notas de versión

Patrones listos para pegar para [help/user-guide/release-notes.md](../../help/user-guide/release-notes.md). Hacer coincidir el tono y la estructura con el archivo que lo rodea.

## Ejemplo mínimo de frontmatter (solo para la nueva página)

Usar solo cuando **se cree** una nueva página de notas de la versión desde cero. Si el archivo ya existe, conserve su contenido principal completo en su lugar.

```yaml
---
title: Adobe GenStudio for Performance Marketing release notes
description: Learn about the latest features and enhancements to Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
role: User
exl-id: 32f5104e-ae15-4092-8a34-642fc641baf9
---
```

## Sección de funciones (con Beta)

```markdown
### Generative Expand AI functionality

[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}

Now, in GenStudio for Performance Marketing [!DNL Create] you can use [Generative Expand AI capabilities](/help/user-guide/create/manage-variants.md#use-generative-expand) to expand the dimensions of images and add generative content to fit your ad templates in paid media variants.
```

## Sección de funciones (vínculo de documentación en prosa)

```markdown
### Compatible assets filter

A new filter in the [!DNL Insights] module automatically hides [unsupported image and video assets](/help/user-guide/insights/ads.md#ad-formats) from ad previews, eliminating visual clutter and broken tiles. This enhancement ensures users only see media that's actually available and ready to use, creating a cleaner and more reliable experience.
```

## Correcciones y mejoras (viñetas)

```markdown
### Fixes and enhancements

* Added support for [publishing ad experiences](/help/user-guide/activation/activate-linkedin-ad.md) from GenStudio for Performance Marketing into LinkedIn Campaign Manager. [!DNL Activate] supports detailed LinkedIn ad previews before publishing to LinkedIn Campaign Manager.
```

Utilice solamente esta subsección para los elementos **explícitamente** etiquetados como corrección o mejora en el material de origen.

## Bloque archivado (Notas de la versión anteriores)

```markdown
+++Notes from 2025.05.15

### Fixes and enhancements

* Enabled functionality for [adding alternative (alt) text](/help/user-guide/create/manage-variants.md#add-alt-text-for-images) to an image for an individual variant.
* Added a [new Meta aspect ratio](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) —Landscape 1.19:1 (1080 pixel width).
* Now you can choose more than one experience for export or download. See [Export experiences](/help/user-guide/content/manage-assets.md#export-experiences).

+++
```
