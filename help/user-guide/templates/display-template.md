---
title: Mostrar directrices de plantillas de publicidad
description: Siga las prácticas recomendadas al utilizar plantillas de anuncios en pantalla y banners con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
source-git-commit: f4bc3442678e6366e185d0c7a91c784d43b8e455
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Mostrar directrices de plantilla de publicidad

Las plantillas de visualización son diseños prediseñados que se utilizan para crear titulares y anuncios de visualización atractivos visualmente. Proporcionan un marco flexible para incorporar imágenes, texto y call to action, lo que garantiza coherencia y eficacia al producir varias variaciones de anuncios. Al preparar la plantilla para utilizarla en GenStudio for Performance Marketing, asegúrese de que todos los recursos estén optimizados para la visualización web y cumplan los formatos y tamaños de archivo necesarios.

Siga estas prácticas recomendadas de diseño al personalizar las plantillas de anuncio de banner y visualización para trabajar con GenStudio for Performance Marketing:

- Usar fuentes Adobe o Google
- Preparar recursos que se muestren bien en dimensiones delgadas
- Se requiere exactamente un campo de imagen
- **no** utiliza imágenes de fondo incrustadas o codificadas
- Usar imágenes de fondo (campo `image`) cargadas al repositorio de contenido de GenStudio for Performance Marketing. Respete las directrices de [Carga de imágenes para anuncios en pantalla](#uploading-images-for-display-ads) para obtener mejores resultados
- **no** usa JavaScript
- Solo se puede utilizar una sección, lo que genera un único conjunto de elementos de plantilla

## Nombres de campo reconocidos

Al personalizar el titular o la plantilla de anuncio en pantalla, utilice marcadores de posición de contenido para los siguientes campos obligatorios:

- `headline`
- `sub_headline`
- `body`
- `image` (obligatorio, seleccionado entre JPEG de contenido, PNG o GIF)

GenStudio for Performance Marketing genera automáticamente los campos siguientes. No es necesario aplicar marcadores de posición de contenido para:

- `cta`

Consulte [Marcadores de posición de contenido](/help/user-guide/content/customize-template.md#content-placeholders) para obtener más información sobre el uso de nombres de campo en las plantillas.

## Dimensiones compatibles

Se debe definir la anchura y la altura (píxeles).

| Orientación | Dimensiones (píxeles) | Notas |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| Vertical | 300 x 600<br>160 x 600 | Común para rascacielos y banners de media página. |
| Horizontal | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | Tamaños estándar de tabla de clasificación, rectángulo medio y banner. |
| Personalizado | 50 x 50 a 2000 x 2000 | Se utiliza para ubicaciones no estándar o únicas; compruebe los límites de la plataforma. |

## Carga de imágenes para anuncios en pantalla

Las imágenes utilizadas en los anuncios en pantalla deben proceder del repositorio de contenido y deben cargarse correctamente para garantizar que la imagen se muestre con precisión en la plantilla.

Cuando una plantilla de visualización incluye una imagen de extremo a extremo (sangrado completo), la imagen seleccionada cambia de tamaño automáticamente para ajustarse a las dimensiones de plantilla completas. Sin embargo, si la imagen no coincide con la proporción de aspecto de la plantilla, la imagen se recorta para ajustarse a las dimensiones de la plantilla y es posible que no se muestre según lo esperado.

No existe la funcionalidad de &quot;ajuste automático&quot; para las imágenes en las plantillas de anuncios en pantalla.

Para resolver el recorte de imágenes, los usuarios deben definir la proporción de aspecto de la imagen en la plantilla cuando se cargue en el repositorio de contenido. Al cargar una plantilla de anuncio en pantalla aprobada:

1. [Continúe con el proceso de carga de plantillas](/help/user-guide/content/use-templates.md#add-a-template) hasta que llegue a la página **[!UICONTROL Agregar detalles]**.

1. Defina la proporción de aspecto de la imagen que se usará en la plantilla en **[!UICONTROL Anchura del anuncio (px)]** y **[!UICONTROL Altura del anuncio (px)]**. Esto define la ventana de imagen para la sección de la plantilla que muestra la imagen.

1. En la sección **[!UICONTROL Más detalles]**, seleccione la lista desplegable **[!UICONTROL Tamaño de imagen]** y elija _Recortar a un tamaño fijo_.
   ![Recortado a un tamaño fijo](./crop-to-fixed-size.png "Recortado a un tamaño fijo"){width="80%"}

Para determinar el tamaño y la proporción de aspecto de una imagen en el explorador:

1. Inspeccione la imagen.
   - Windows/Linux:
      - Presione F12.
   - macOS:
      - Pulse Comando + Opción + I.

1. Pase el ratón sobre la imagen.

1. Observe la relación de aspecto. Utilícelo para definir la proporción de aspecto de la imagen en la plantilla.

Cuando estos detalles no se aplican durante la carga, se asume que la imagen es toda la proporción de aspecto de la plantilla y las imágenes que no coinciden exactamente con esa proporción de aspecto aparecerán recortadas.

![Imagen recortada en un anuncio en pantalla](./cropped-display.png "Recorte de imagen"){width="60%"}

**❌Se recortó la imagen en una plantilla de anuncio en pantalla**

![Imagen mostrada en un anuncio en pantalla](./full-fit.png "Imagen mostrada en el anuncio en pantalla"){width="60%"}

**✅imagen completamente mostrada**
