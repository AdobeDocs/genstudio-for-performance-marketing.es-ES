---
title: Directrices de plantilla de LinkedIn
description: Siga las prácticas recomendadas al utilizar plantillas de LinkedIn con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 85432185-8311-411b-b57b-f482c3d45854
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 2%

---

# Directrices de plantilla de LinkedIn

Las plantillas de LinkedIn proporcionan una forma estructurada de crear y personalizar anuncios creativos para campañas de LinkedIn. Estas directrices garantizan que los anuncios cumplan las especificaciones de LinkedIn y, al mismo tiempo, optimizan el proceso creativo en GenStudio for Performance Marketing. Esta guía le ayuda a prepararse para una promoción de la marca coherente y un rendimiento eficaz en todas las plataformas móviles y de escritorio de LinkedIn.

Siga estas prácticas recomendadas de diseño al personalizar las plantillas de anuncios de LinkedIn para que funcionen con GenStudio for Performance Marketing:

- Se requiere exactamente un campo de imagen
- Tamaño máximo de imagen de 5 MB
- Titular máximo de 70 caracteres
- Texto introductorio máximo de 150 caracteres
- Solo se puede utilizar una sección, lo que genera un único conjunto de elementos de plantilla

## Nombres de campo reconocidos

Al personalizar la plantilla de LinkedIn, aplique marcadores de posición de contenido para estos campos obligatorios:

- `image` (obligatorio, seleccionado entre JPEG de contenido, PNG o GIF)
- `on_image_text` (texto que aparece sobre la imagen)

GenStudio for Performance Marketing genera automáticamente los campos siguientes. No es necesario aplicar marcadores de posición de contenido para:

- `headline`
- `introductory_text`
- `cta` (Call to action)

Consulte [Marcadores de posición de contenido](/help/user-guide/content/customize-template.md#content-placeholders) para obtener más información sobre el uso de nombres de campo en las plantillas.

## Proporciones de aspecto admitidas

| Proporción de aspecto | Plataforma | Tamaño mínimo (px) | Tamaño máximo (px) | Notas |
|-------------------|-----------------|---------------|----------------|-------------------------------------------------------------------------------------|
| Cuadrado 1:1 | Escritorio, Móvil | 360 x 360 | 4320 x 4320 | Muy versátil. Ideal para lograr una apariencia uniforme en todos los dispositivos y ubicaciones. |
| Horizontal 1.91:1 | Escritorio | 640 x 360 | 7680 x 4320 | Formato horizontal estándar. Se utiliza comúnmente para contenido patrocinado y anuncios de fuentes de noticias. |
| Vertical 1:1.91 | Dispositivo móvil | 360 x 640 | 2430 x 4320 | Formato vertical alto. Optimizado para la visualización móvil, que ofrece más presencia en la pantalla. |
| Vertical 2:3 | Dispositivo móvil | 360 x 640 | 2430 x 4320 | Un poco menos alto que 1:1.91. Ideal para campañas con prioridad móvil. |
| Vertical 4:5 | Dispositivo móvil | 360 x 640 | 2430 x 4320 | Recomendado para dispositivos móviles. Equilibra la visibilidad y el contenido, lo que a menudo produce un mayor impacto. |

<!-- Potentially add an example

## Template example

+++Example: LinkedIn template

+++

-->
