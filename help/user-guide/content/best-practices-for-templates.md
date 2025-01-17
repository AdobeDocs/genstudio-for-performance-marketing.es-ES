---
title: Prácticas recomendadas para plantillas
description: Siga las prácticas recomendadas al utilizar plantillas con Adobe GenStudio for Performance Marketing.
feature: Templates, Content
last-substantial-update: 2024-12-13T00:00:00Z
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: 9cc284cdb00a204baf6b0a2d9d7f67cf9bc9c81f
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 0%

---

# Prácticas recomendadas para usar plantillas

Las plantillas reducen significativamente el tiempo y el esfuerzo necesarios para generar contenido nuevo al proporcionar un punto de partida que incluye diseños y elementos de diseño preconfigurados.

Utilice las siguientes recomendaciones cuando utilice plantillas con GenStudio for Performance Marketing:

1. Obtenga información sobre [elementos de plantilla](#know-about-template-elements)
1. Configure [directrices de canal](#configure-channel-guidelines) para una personalización efectiva del contenido
1. Diseñe con [estándares de accesibilidad](accessibility-for-templates.md) para obtener una experiencia óptima
1. Seguir [directrices de plantillas específicas de canal](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>Obtenga más información acerca de los elementos y procedimientos básicos de la plantilla en [Trabajar con plantillas](use-templates.md). Y profundiza en [la personalización de una plantilla](customize-template.md) para usarla en tu próxima campaña.

## Información sobre los elementos de plantilla

Como práctica recomendada, familiarícese con las partes de una plantilla. Cada tipo de plantilla utiliza diferentes elementos para crear una estructura para la creación de contenido específica del canal. Para personalizar la plantilla, utilice los nombres de campo en lugar de estos elementos donde necesite que GenStudio for Performance Marketing genere contenido.

Ver [elementos de plantilla](use-templates.md#template-elements).

## Configuración de directrices de canal

Configure las directrices de canal para cada marca antes de usar las plantillas en GenStudio for Performance Marketing. Las directrices de canal influyen directamente en el tipo de contenido generado al utilizar la plantilla. Por ejemplo, puede establecer límites de caracteres en el cuerpo de un correo electrónico.

![Especificaciones del cuerpo](/help/assets/channel-email-body.png)

Consulte [directrices de canal](/help/user-guide/guidelines/brands.md#channel-guidelines).

## Siga las directrices de plantillas específicas del canal

Cree plantillas que se adapten al diseño y a los requisitos visuales de cada canal. Tenga en cuenta las siguientes sugerencias y restricciones al trabajar con cada tipo de plantilla para garantizar un rendimiento y una compatibilidad óptimos:

>[!BEGINTABS]

>[!TAB Correo electrónico]

Siga estas prácticas recomendadas de diseño al personalizar las plantillas de correo electrónico para que funcionen con GenStudio for Performance Marketing:

- Usar fuentes de Adobe o Google
- Utilizar HTML limpio y adaptable y CSS en línea
- **no** usa JavaScript
- **no** usa ancho fijo en el cuerpo o contenedor
- **no** usa la codificación base64 para las imágenes porque puede aumentar significativamente el tamaño de la plantilla

**Restricciones**:

- Uso de [secciones](customize-template.md#sections-or-groups):
   - Una plantilla básica (solo una sección) puede generar un único conjunto de elementos de plantilla.
   - Una plantilla compleja (varias secciones) puede generar hasta tres conjuntos de elementos de plantilla.
- Los campos máximos permitidos en una plantilla son 20
- El tamaño máximo de archivo de HTML es 102 KB

**Nombres de campo reconocidos**:

Para el correo electrónico, el campo `subject` se incluye automáticamente. Utilice marcadores de posición de contenido para los siguientes campos:

- `pre_header`
- `headline`
- `body`
- `cta`
- `image` (seleccionado de Contenido)
- `brand_logo`

Consulte [Marcadores de posición de contenido](customize-template.md#content-placeholders) para obtener más información sobre el uso de nombres de campo en las plantillas.

>[!TAB Meta anuncio]

Siga estas prácticas recomendadas de diseño al personalizar las plantillas de publicidad meta para que funcionen con GenStudio for Performance Marketing:

- Utilizar una anchura de 360 píxeles para los diseños de columna
- Utilice una resolución mínima de 1080 x 1080 píxeles para las imágenes
- **no** usa un tamaño de fuente relativo
- **no** define ventanillas móviles
- **no** usa JavaScript
- **no** reemplaza un elemento HTML en CSS
- Utilice la siguiente configuración para las imágenes de fondo:

  Agregar el valor `object-fit: cover` a la clase CSS `background-image`:

  ```css
  .background-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  ```

**Restricciones**:

- Uso de [secciones](customize-template.md#sections-or-groups):
   - Solo se puede utilizar una sección, lo que genera un único conjunto de elementos de plantilla.

**Proporciones de aspecto compatibles**:

- Cuadrado 1:1 (1080 x 1080 píxeles)
- Vertical 4:5 (1080 x 1350 píxeles)
- Historia 9:16 (1080 x 1920 píxeles)
- Tamaño de imagen personalizado: (anchura mínima de imagen de 50 x 50 píxeles)

**Nombres de campo reconocidos**:

Para los anuncios Meta, los campos `headline`, `body` y `CTA` se generan automáticamente. Utilice marcadores de posición de contenido para los siguientes campos:

- `image` (seleccionado de Contenido)
- `on-image-text`
- `brand_logo`

Consulte [Marcadores de posición de contenido](customize-template.md#content-placeholders) para obtener más información sobre el uso de nombres de campo en las plantillas.

>[!TAB Anuncio de visualización]

[!BADGE Beta]{type=Informative tooltip="Esta función se encuentra actualmente en Beta, por lo que algunas funciones pueden estar limitadas o sujetas a cambios."}

Siga estas prácticas recomendadas de diseño al personalizar las plantillas de anuncios en pantalla para trabajar con GenStudio for Performance Marketing:

- Usar fuentes de Adobe o Google
- Preparar recursos que se muestren bien en dimensiones delgadas
- **no** utiliza imágenes de fondo incrustadas o codificadas
- Usar imágenes de fondo (campo `image`) cargadas al repositorio de contenido de GenStudio for Performance Marketing
- **no** usa JavaScript

**Restricciones**:

- Uso de [secciones](customize-template.md#sections-or-groups):
   - Solo se puede utilizar una sección, lo que genera un único conjunto de elementos de plantilla.

**Dimensiones compatibles**:

- Vertical: (píxeles)
   - 300 x 600
   - 160 x 600 &#x200B;
- Horizontal: (píxeles)
   - 300 x 250
   - 728 x 90
   - 336 x 280
   - 320 x 50
   - 970 x 250 &#x200B;
- Personalizado: (píxeles)
   - 50 x 50 a 2000 x 2000

**Nombres de campo reconocidos**:

Utilice marcadores de posición de contenido para los siguientes campos:

- `headline`
- `body`
- `cta`
- `image` (seleccionado de Contenido)

Consulte [Marcadores de posición de contenido](customize-template.md#content-placeholders) para obtener más información sobre el uso de nombres de campo en las plantillas.

>[!ENDTABS]
