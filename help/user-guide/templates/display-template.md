---
title: Mostrar directrices de plantilla de publicidad
description: Siga las prácticas recomendadas al utilizar plantillas de anuncios en pantalla y banners con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
source-git-commit: 78313c2a2177a2ccb39e37a87ca3c657e7906d0a
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 1%

---

# Mostrar directrices de plantilla de publicidad

Las plantillas de visualización son diseños prediseñados que se utilizan para crear titulares y anuncios de visualización atractivos visualmente. Proporcionan un marco flexible para incorporar imágenes, texto y call to action, lo que garantiza coherencia y eficacia al producir varias variaciones de anuncios. Al preparar la plantilla para utilizarla en GenStudio for Performance Marketing, asegúrese de que todos los recursos estén optimizados para la visualización web y cumplan los formatos y tamaños de archivo necesarios.

Siga estas prácticas recomendadas de diseño al personalizar las plantillas de anuncio de banner y visualización para trabajar con GenStudio for Performance Marketing:

- Usar fuentes Adobe o Google
- Preparar recursos que se muestren bien en dimensiones delgadas
- Se requiere exactamente un campo de imagen
- **no** utiliza imágenes de fondo incrustadas o codificadas
- Usar imágenes de fondo (campo `image`) cargadas al repositorio de contenido de GenStudio for Performance Marketing
- **no** usa JavaScript
- Solo se puede utilizar una sección, lo que genera un único conjunto de elementos de plantilla

## Nombres de campo reconocidos

Para los titulares y anuncios en pantalla, GenStudio for Performance Marketing genera automáticamente el campo `cta`. Al personalizar la plantilla, utilice marcadores de posición de contenido para los siguientes campos obligatorios:

- `headline`
- `sub_headline`
- `body`
- `image` (obligatorio, seleccionado entre JPEG de contenido, PNG o GIF)

Consulte [Marcadores de posición de contenido](/help/user-guide/content/customize-template.md#content-placeholders) para obtener más información sobre el uso de nombres de campo en las plantillas.

## Dimensiones compatibles

Se debe definir la anchura y la altura (píxeles).

| Orientación | Dimensiones (píxeles) | Notas |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| Vertical | 300 x 600<br>160 x 600 | Común para rascacielos y banners de media página |
| Horizontal | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | Tamaños estándar de clasificación, rectángulo medio y banner |
| Personalizado | 50 x 50 a 2000 x 2000 | Se utiliza para ubicaciones no estándar o únicas; compruebe los límites de la plataforma |

<!-- Potentially add an example

## Template example

+++Example: Display ad template

+++

-->
