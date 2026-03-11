---
title: Directrices de plantilla de LinkedIn
description: Siga las prácticas recomendadas al utilizar plantillas de LinkedIn con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 85432185-8311-411b-b57b-f482c3d45854
TQID: https://experienceleague.adobe.com/YyG3WuMkdVAaACX03qLKzzw-fFA3WfT9K2ohjnQNPcI
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 242ab858144fd152fd55645143f869fddf7b6fe0
workflow-type: tm+mt
source-wordcount: 287
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

Consulte [Marcadores de posición de contenido](/help/user-guide/templates/customize-template.md#content-placeholders) para obtener más información sobre el uso de nombres de campo en las plantillas.

## Proporciones de aspecto admitidas

Todas las anchuras de las plantillas de LinkedIn están codificadas a 1200 píxeles.

| Proporción de aspecto | Plataforma | Dimensiones (px) | Notas |
|-------------------|-----------------|------------|-------------------------------------------------------------------------------------|
| Cuadrado 1:1 | Escritorio, Móvil | 1200 x 1200 | Muy versátil. Ideal para lograr una apariencia uniforme en todos los dispositivos y ubicaciones. |
| Horizontal 1.91:1 | Escritorio | 1200 x 628 | Formato horizontal estándar. Se utiliza comúnmente para contenido patrocinado y anuncios de fuentes de noticias. |
| Vertical 1:1.91 | Dispositivo móvil | 1200 x 2292 | Formato vertical alto. Optimizado para la visualización móvil, que ofrece más presencia en la pantalla. |
| Vertical 2:3 | Dispositivo móvil | 1200 x 1800 | Un poco menos alto que 1:1.91. Ideal para campañas con prioridad móvil. |
| Vertical 4:5 | Dispositivo móvil | 1200 x 1500 | Recomendado para dispositivos móviles. Equilibra la visibilidad y el contenido, lo que a menudo produce un mayor impacto. |

<!-- 
Potentially add an example

## Template example

+++Example: LinkedIn template

+++

-->
