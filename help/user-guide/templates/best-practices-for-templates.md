---
title: Prácticas recomendadas para plantillas
description: Siga las prácticas recomendadas al utilizar plantillas con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: 71b46454fa6fe2037ea6b103c0dfeedad74b8919
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Prácticas recomendadas para usar plantillas

Las plantillas reducen significativamente el tiempo y el esfuerzo necesarios para generar contenido nuevo al proporcionar un punto de partida que incluye diseños y elementos de diseño preconfigurados.

Siga las siguientes recomendaciones al utilizar plantillas con GenStudio for Performance Marketing:

1. Obtenga información sobre [elementos de plantilla](#know-about-template-elements)
1. Configure [directrices de canal](#configure-channel-guidelines) para una personalización efectiva del contenido
1. Diseñe con [estándares de accesibilidad](accessibility-for-templates.md) para obtener una experiencia óptima
1. Seguir [directrices de plantillas específicas de canal](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>Conozca los conceptos básicos de los elementos y procedimientos de plantilla en [Trabajar con plantillas](use-templates.md). Y profundiza en [la personalización de una plantilla](customize-template.md) para obtener instrucciones específicas que puedes usar en tu próxima campaña.

## Uso de los elementos de plantilla adecuados

Cada tipo de plantilla utiliza diferentes elementos para crear una estructura para la creación de contenido específica del canal. [Familiarícese con las partes de una plantilla](use-templates.md#template-elements) e incluya los mejores elementos para su contenido y tipo de plantilla.

Al personalizar la plantilla, utilice los nombres de campo en lugar de estos elementos donde necesite que GenStudio for Performance Marketing genere contenido.

Ver [elementos de plantilla](use-templates.md#template-elements).

## Uso de texto de marcador de posición en plantillas

El texto de marcador de posición puede ayudar a definir la sintaxis o la estructura del contenido que un usuario debe rellenar posteriormente en una plantilla. Por ejemplo, {first_name}.{last_name}@email.etc. para definir una dirección de correo electrónico. Sin embargo, algunos delimitadores comunes ya están reservados para otros significados en GenStudio for Performance Marketing:

❌ &lt; >: en uso para etiquetas de HTML.
❌ {{ }}{{ }} - En uso para expresiones Handlebar.

Utilice corchetes sencillos (rectos o curvos) para indicar el texto del marcador de posición y evitar confusiones con las etiquetas existentes.

✅ {first_name} - Marcador de posición para el nombre.

## Configuración de directrices de canal

Definir directrices de canal claras es esencial para garantizar que el contenido generado se ajuste a los requisitos y objetivos de la marca. Las directrices de canal permiten especificar reglas para elementos como el tono, la longitud y el estilo que se utilizan en la plantilla. Por ejemplo, puede establecer un recuento máximo de caracteres para el cuerpo o requerir un estilo call-to-action específico. Al establecer estas directrices por adelantado, reduce la necesidad de escribir instrucciones detalladas en cada mensaje de IA, lo que optimiza el proceso de generación de contenido y garantiza la coherencia en los correos electrónicos.

Revise y defina las [directrices de canal](/help/user-guide/guidelines/brands.md#channel-guidelines) de su marca para todos los campos clave de su plantilla. Si no define directrices, se aplican las [directrices predeterminadas para canales](/help/user-guide/guidelines/brands.md#default-channel-guidelines), que pueden no reflejar completamente los requisitos de su marca.

![Especificaciones del cuerpo](/help/assets/channel-email-body.png)

Conozca de qué manera las [directrices de marcas, productos y personas](/help/user-guide/guidelines/overview.md) influyen en el contenido generado y cómo adaptarlo a sus objetivos de marketing.

## Carga de imágenes para plantillas

Las imágenes utilizadas en las plantillas deben proceder del repositorio de contenido y deben cargarse correctamente para garantizar que la imagen se muestre con precisión.

Cuando una plantilla incluye una imagen de extremo a extremo (sangrado completo), la imagen seleccionada cambia de tamaño automáticamente para ajustarse a las dimensiones completas de la plantilla. Sin embargo, si la imagen no coincide con la proporción de aspecto de la plantilla, la imagen se recorta para ajustarse a las dimensiones de la plantilla y es posible que no se muestre según lo esperado.

No hay funcionalidad de &quot;autoajuste&quot; para las imágenes incluidas en las plantillas.

Para resolver el recorte de imágenes, los usuarios deben definir la proporción de aspecto de la imagen que se utilizará en la plantilla cuando se cargue en el repositorio de contenido. Al cargar una plantilla aprobada:

1. [Continúe con el proceso de carga de plantillas](/help/user-guide/templates/use-templates.md#add-a-template) hasta que llegue a la página **[!UICONTROL Agregar detalles]**.

2. Defina la proporción de aspecto de la imagen que se usará en la plantilla en **[!UICONTROL Anchura del anuncio (px)]** y **[!UICONTROL Altura del anuncio (px)]**. Esto define la ventana de imagen para la sección de la plantilla que muestra la imagen.

3. En la sección **[!UICONTROL Más detalles]**, seleccione la lista desplegable **[!UICONTROL Tamaño de imagen]** y elija _Recortar a un tamaño fijo_.
   ![Recortado a un tamaño fijo](images/crop-to-fixed-size.png "Recortado a un tamaño fijo"){width="80%"}

Para determinar el tamaño y la proporción de aspecto de una imagen en el explorador:

1. Inspeccione la imagen.
   - En Windows/Linux:
      - Presione F12.
   - En macOS:
      - Pulse Comando + Opción + I.

1. Pase el ratón sobre la imagen.

1. Observe la relación de aspecto. Utilícelo para definir la proporción de aspecto de la imagen en la plantilla.

Cuando estos detalles no se aplican durante la carga, se asume que la imagen es toda la proporción de aspecto de la plantilla y las imágenes que no coinciden exactamente con esa proporción de aspecto aparecerán recortadas.

![Imagen recortada en un anuncio en pantalla](images/cropped-display.png "Recorte de imagen"){width="60%"}

**❌Se recortó la imagen en una plantilla de anuncio en pantalla**

![Imagen mostrada en un anuncio en pantalla](images/full-fit.png "Imagen mostrada en el anuncio en pantalla"){width="60%"}

**✅imagen completamente mostrada**

## Siga las directrices de plantillas específicas del canal

Al crear plantillas, asegúrese de que cumplen los requisitos específicos del canal al que va dirigido. Cree plantillas que se adapten al diseño y a los requisitos visuales de cada canal. Existen directrices generales que se aplican a cualquier plantilla, como:

- Utilizar HTML y CSS en línea limpios y adaptables
- Usar fuentes Adobe o Google
- **no** usa JavaScript

{{note-css-effects}}

Consulte más sugerencias y restricciones al trabajar con cada tipo de plantilla para garantizar un rendimiento óptimo:

- [Correos electrónicos](/help/user-guide/templates/email-template.md)
- [Publicidad en pantalla y banner](/help/user-guide/templates/display-template.md)
- [LinkedIn](/help/user-guide/templates/linkedin-template.md)
- [Anuncios de Meta](/help/user-guide/templates/meta-template.md)
