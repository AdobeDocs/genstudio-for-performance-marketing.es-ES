---
title: Resumen de atributos
description: Obtenga información sobre cómo evaluar el rendimiento de atributos específicos en Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Content Attributes, Content Performance
exl-id: 9d05c128-50d5-415a-ae60-7023c36c06ad
source-git-commit: 8a5d15df7a347c4ee7767610fc9bb23fc7b71db4
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---

# Resumen de atributos

La vista [!DNL Insights] _[!UICONTROL Atributos]_ muestra una lista de atributos utilizados en campañas publicitarias para la cuenta de canal seleccionada.

{{connect-insights}}

La tabla _[!UICONTROL Attributes]_ está organizada con el nombre [!UICONTROL Attribute]. Puede alternar entre los tipos de lista usando el botón **[!UICONTROL Imágenes]** y el botón **[!UICONTROL Vídeo]**. Haga clic en el icono de configuración (cog) situado encima de la parte derecha de la tabla para alternar las columnas visibles.

El icono de filtro (canal) situado encima de la parte izquierda de la tabla abre el menú **[!UICONTROL Filtro]**, en el que puede seleccionar entre varias listas. Seleccione **[!UICONTROL Borrar todo]** sobre la tabla para eliminar todos los filtros.

![Filtro y tabla de atributos](/help/assets/insights-attributes-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## Detalles del atributo

Los atributos ayudan a identificar [media](media.md#media-details) por sus detalles inherentes, como color, composición, elementos visuales y otras propiedades.

En la vista de detalles del atributo, puede ver qué anuncios utilizan el atributo seleccionado. Los detalles incluyen el rendimiento total de los atributos y un desglose de las métricas de rendimiento relacionadas con cada anuncio.

![Métricas de rendimiento de atributos](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing detecta determinadas funciones y aplica el atributo adecuado al contenido de los medios o al anuncio como etiqueta. Consulte [Categorías](#categories) para ver ejemplos de estas etiquetas. Para ver todos los atributos asociados con un anuncio, haga clic en el icono de configuración (cog) situado encima de la parte derecha de la tabla para seleccionar la columna **[!UICONTROL Attributes]**.

## Categorías

Un atributo _category_ es un grupo de clasificación que organiza atributos relacionados que comparten una característica común. Estas categorías ayudan a optimizar el descubrimiento, la identificación y la comprensión de atributos específicos al proporcionar un mayor contexto y facilitar su aplicación y uso.

GenStudio for Performance Marketing usa la IA y las capacidades de aprendizaje automático de Adobe para estudiar [imágenes](image-features.md), [vídeos](video-features.md), y texto y aplicar [!UICONTROL atributos de medios] según la probabilidad de que sean correctos.

La lista de atributos detectados para el contenido de medios no es exhaustiva. Los medios que contienen un conjunto completo de funciones pueden limitarse a las tres funciones más dominantes identificadas por la API. Por ejemplo, la siguiente ilustración contiene varios atributos de imagen detectados, incluidos varios objetos, colores de primer plano y de fondo.

![atributos de imagen](/help/assets/category/asset-attributes.png "La imagen de Toucan incluye varios atributos detectados"){width="300" zoomable="yes"}

>[!INFO]
>
>No se pueden editar las etiquetas que se detectan y aplican automáticamente.

## Rendimiento de atributos

Las métricas de perspectivas pueden ayudarle a evaluar qué atributos inspiran una mayor participación del cliente.

La siguiente tabla proporciona definiciones y perspectivas para métricas clave de marketing digital en la vista de tabla de [!UICONTROL Atributos]. Cada métrica incluye una breve definición en relación con los atributos, cómo se calcula la métrica y una o más perspectivas para ayudar a comprender su importancia e impacto en una campaña publicitaria.

| Métrica | Definición | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Atributo]** | El nombre del atributo. | Ordene la tabla haciendo clic en el encabezado de la columna de cualquiera de las métricas clave. |
| **[!UICONTROL Category]** | [category](#categories) que representa la calidad inherente de un atributo. |  |
| **[!UICONTROL # de imágenes]** | El número de imágenes que tienen este atributo. | El recuento de la tabla Atributos puede ser diferente al recuento de la vista Detalles del atributo. Esta discrepancia puede producirse si el origen del canal, como Meta y GenStudio, utiliza cálculos de resumen ligeramente diferentes. |
| **[!UICONTROL # de vídeos]** | El número de vídeos que tienen este atributo. | El recuento de la tabla Atributos puede ser diferente al recuento de la vista Detalles del atributo. Esta discrepancia puede producirse si el origen del canal, como Meta y GenStudio, utiliza cálculos de resumen ligeramente diferentes. |
| **[!UICONTROL Impresiones]** | Un recuento de cada vez que una imagen o vídeos con este atributo se cargan en el canal, independientemente de la interacción o visualización. | Un recuento alto de impresiones puede indicar una visibilidad amplia, pero para obtener una verdadera perspectiva de rendimiento, considérala en relación con otras métricas de participación. |
| **[!UICONTROL Clics]** | La cantidad de veces que los usuarios interactúan con una imagen o un vídeo con este atributo. | Un alto número de clics indica un fuerte interés y participación en el contenido, que puede ser eficaz y llegar a la audiencia adecuada. |
| **[!UICONTROL tasa de pulsaciones ]**<br>_CTR_ | Porcentaje (%) de impresiones que generaron clics en imágenes o vídeos con este atributo.<br>**Cálculo**: `clicks` dividido por `impressions` | Una alta tasa de clics indica que el contenido es muy relevante y motivador para la audiencia en cuanto a mensajería y diseño, y que se dirige de manera efectiva a los intereses de la audiencia. |
| **[!UICONTROL CPM ]**<br>_Costo por mil_ | Coste por cada mil impresiones de publicidad de una imagen o vídeo con este atributo.<br>**Cálculo**: importe total `spent` dividido por alcance y luego multiplicado por 1000 | Un valor bajo puede indicar una visibilidad rentable, especialmente cuando se asocia con una tasa de pulsaciones alta. |
| **[!UICONTROL CPA ]**<br>_Costo por acción_ | Coste promedio empleado para lograr una acción específica del cliente, como una compra o suscripción.<br>**Cálculo**: importe total `spent` dividido por el número de acciones del cliente completadas | Ayuda a identificar atributos que resultan en acciones valiosas del cliente. |
| **[!UICONTROL CPC ]**<br>_Costo por clic_ | Coste medio asociado con cada clic en imágenes o vídeos con este atributo.<br>**Cálculo**: importe total `spent` dividido entre `clicks` | Unos costes medios menores pueden indicar un gasto publicitario rentable, especialmente en comparación con un aumento de las conversiones. |
| **[!UICONTROL Gasto]** | El importe gastado del presupuesto en relación con los atributos durante un período de tiempo determinado. | Un gasto elevado en un período corto puede indicar un uso rápido, lo que podría dar lugar a un agotamiento prematuro de los recursos. Realice un seguimiento de la cantidad gastada con respecto a las métricas de rendimiento clave para ayudar a monitorizar la rentabilidad general de la inversión. |
