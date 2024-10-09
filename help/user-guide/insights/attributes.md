---
title: Resumen de atributos
description: Obtenga información sobre cómo evaluar el rendimiento de atributos específicos en Adobe GenStudio for Performance Marketing.
feature: Insights, Assets
source-git-commit: ce08231cb723bec3d80a732837b72a435d3b552d
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# Resumen de atributos

La vista [!DNL Insights] _[!UICONTROL Atributos]_ muestra una lista de atributos utilizados en campañas publicitarias para la cuenta de canal seleccionada.

La tabla _[!UICONTROL Attributes]_ está organizada con el nombre [!UICONTROL Attribute]. Puede alternar entre los tipos de lista usando el botón **[!UICONTROL Imágenes]** y el botón **[!UICONTROL Vídeo]**. Haga clic en el icono de configuración (cog) situado encima de la parte derecha de la tabla para alternar las columnas visibles.

El icono de filtro (canal) situado encima de la parte izquierda de la tabla abre el menú **[!UICONTROL Filtro]**, en el que puede seleccionar entre [!UICONTROL Cuenta] y [!UICONTROL Categoría de atributos] para filtrar los atributos de la tabla. El ejemplo siguiente muestra una lista de atributos en la categoría `Lighting Condition`.

![Filtro y tabla de atributos](/help/assets/insights-attributes-filter.png){zoomable="yes"}

## Detalles del atributo

Los atributos ayudan a identificar los recursos por sus detalles inherentes, como el color, la composición, los elementos visuales y otras propiedades.

En la vista de detalles del atributo, puede ver qué experiencias utilizan el atributo seleccionado. Los detalles incluyen el rendimiento total de los atributos y un desglose de las métricas de rendimiento relacionadas con cada experiencia.

![Métricas de rendimiento de atributos](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing detecta determinadas funciones y aplica el atributo adecuado a un recurso o experiencia como etiqueta. Vea [Categorías](#categories) para ver ejemplos de estas etiquetas. Para ver todos los atributos asociados a una experiencia, haga clic en el icono de configuración (cog) situado encima de la parte derecha de la tabla para seleccionar la columna **[!UICONTROL Atributos]**.

## Categorías

GenStudio for Performance Marketing reconoce determinadas funciones de imágenes, vídeos y texto, y aplica una etiqueta de características al recurso. Una _categoría_ es un conjunto de características que comparten una característica específica. Un valor de ejemplo de _orientación de la imagen_ es `landscape`.

Los atributos detectados y aplicados automáticamente no se pueden editar.

<!--
Select any of the following to open a detailed list of feature categories:

+++**Image features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Background Colors      | 14 colors |
| Camera Position        | - `low angle`, `high angle`, `dutch angle`<br>- `overhead view`, `eye level`,`bird's eye view` |
| Camera Proximity       | `close up`, `mid shot`, `long shot` |
| Camera Setting         | - `fast shutter speed`, `long exposure`, `double exposure`<br>- `normal mode`, `flash`, `macro`, `wide-angle`<br>- `black and white`, `surreal`<br>- `bokeh blur`, `motion blur`, `tilt-shift blur` |
| Foreground Colors      | 14 colors |
| Image Type             | `photograph`, `sketch`, `painting`, `digital cartoon`, `infographics`, `graphic design`, `collage`, `screenshot` |
| Lighting Condition     | golden hour, blue hour, midday, overcast, night, high-key, low-key, daylight, incandescent, fluorescent, colorful, studio |
| Objects                | The items, entities, and elements that are visible, such as `lighthouse`, `orchid`, or `tunnel`. |
| Orientation            | Examples: `landscape`, `portrait`, `square` |
| Overall Tone           | `warm`, `cool`, `neutral` |
| People Categories      | Examples: `person`, `social group`, `people`, `kid` |
| Photography Styles     | `aerial photography`, `aerial photography`, `architectural photography`, `astrophotography`, `black and white photography`, `business photography`, `cityscape photography`, `commercial photography`, `composite photography`, `creative photography`, `editorial photography`, `event photography`, `family photography`, `fashion photography`, `fine art photography`, `food photography`, `holiday photography`, `indoor photography`, `landscape photography`, `lifestyle photography`, `macro photography`, `minimalist photography`, `night photography`, `outdoor photography`, `pet photography`, `portrait photography`, `product photography`, `real estate photography`, `seascape photography`, `sports photography`, `still-life photography`, `street photography`, `travel photography`, `underwater photography`, `wildlife photography` |
| Scenes                 | Examples: `city`, `island`, `living room` |
| Tags                   | Examples: `gaming`, `law`, `yoga` |
| Visual Attention Spread| The level of viewer attention spread across an image: `high`, `low` |
| Visual Content Density | The amount of information or detail in an image: `high`, `low` |

+++

+++**Video features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Audio Genre  | |
| Audio Genre Category  | |
| Audio Mood  | |
| Audio Types| |
| Objects  | |
| Orientation  | |
| People Categories  | |
| Scenes  | |
| Styles  | |
| Tags   | |
| Video Category  | |
| Video Type  | |

+++

+++**Text features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Emojis Count  | |
| HashTags Count  | |
| Keywords  | |
| Marketing Emotions  | |
| Narratives  |  |
| Persuasion Strategies  |  |
| Readability  | |
| Sentences Count  | |
| Stop Words Ratio  | |
| Text Quotes Count  | |
| Tones  | |
| Words Count  | |
| Words Count Per Sentence  | |

+++

-->

## Métricas de atributo

Las métricas de perspectivas pueden ayudarle a evaluar qué atributos inspiran una mayor participación del cliente.

### Detalles de métricas

La siguiente tabla proporciona definiciones y perspectivas para métricas clave de marketing digital en la vista [!UICONTROL Atributos]. Cada métrica incluye una breve definición en relación con un recurso, cómo se calcula la métrica y una o más perspectivas para ayudar a comprender su importancia e impacto en una campaña publicitaria.

| Métrica | Definición | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Atributo]** | El nombre del atributo. | Ordene la tabla haciendo clic en el encabezado de la columna de cualquiera de las métricas clave. |
| **[!UICONTROL Categoría]** | [category](#categories) que representa la calidad inherente de un atributo. |  |
| **[!UICONTROL # de imágenes]** | Un recuento de imágenes con este atributo. |  |
| **[!UICONTROL # de vídeos]** | Un recuento de vídeos con este atributo. |  |
| **[!UICONTROL Impresiones]** | Un recuento de cada vez que una imagen o vídeos con este atributo se cargan en el canal, independientemente de la interacción o visualización. | Un recuento alto de impresiones puede indicar una visibilidad amplia, pero para obtener una perspectiva de rendimiento real, considere la posibilidad de con otras métricas de participación. |
| **[!UICONTROL Clics]** | Número de veces que los usuarios interactúan con una imagen o un vídeo con este atributo. | Un alto número de clics indica un fuerte interés y participación en el contenido, que puede ser eficaz y llegar a la audiencia adecuada. |
| **[!UICONTROL tasa de pulsaciones ]**<br>_CTR_ | Porcentaje (%) de impresiones que generaron clics en imágenes o vídeos con este atributo.<br>**Cálculo**: `clicks` dividido por `impressions` | Una alta tasa de clics indica que el contenido es muy relevante y motivador para la audiencia en cuanto a mensajería y diseño, y que se dirige de manera efectiva a los intereses de la audiencia. |
| **[!UICONTROL CPM ]**<br>_Costo por mil_ | Costo ($) por cada mil impresiones de publicidad de una imagen o vídeo con este atributo.<br>**Cálculo**: importe total `spent` dividido por alcance y luego multiplicado por 1000 | Un valor bajo puede indicar una visibilidad rentable, especialmente cuando se asocia con una tasa de pulsaciones alta. |
| **[!UICONTROL CPC ]**<br>_Costo por clic_ | Coste medio ($) asociado con cada clic en imágenes o vídeos con este atributo.<br>**Cálculo**: importe total `spent` dividido entre `clicks` | Unos costes medios menores pueden indicar un gasto publicitario rentable, especialmente en comparación con un aumento de las conversiones. |
| **[!UICONTROL Gasto]** | La cantidad ($) gastada del presupuesto en relación con los atributos durante un período de tiempo determinado. | Un gasto elevado en un período corto puede indicar un uso rápido, lo que podría dar lugar a un agotamiento prematuro de los recursos. Realice un seguimiento de la cantidad gastada con métricas de rendimiento clave para ayudar a monitorizar la rentabilidad general de la inversión. |
