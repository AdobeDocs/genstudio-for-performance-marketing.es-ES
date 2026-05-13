---
title: Resumen de atributos
description: Obtenga información sobre cómo evaluar el rendimiento de atributos específicos en Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Content Attributes, Content Performance
exl-id: 9d05c128-50d5-415a-ae60-7023c36c06ad
TQID: https://experienceleague.adobe.com/FW4WpVLALtYYI2mGT3i3IH5KYuYnZ5h2pbnm9gKcrVE
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7id: c95c94c1-727b-457a-9184-a4dda4c95ab2id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f321b88b-6bb7-49cc-a16a-ae2b665ebd32
subfeature_v2: id: a98e0185-3180-4e8c-8f31-f72af4cc21a2id: b03d2162-d906-40a0-9cbd-001391e22d4a
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: b5520579-b31f-4df7-9281-f0d9f91e2edcid: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eb30f47f-d87a-400f-8f78-63ce7979ff56
source-git-commit: c9b8177a564cfcdfd2b63cd28fa22eb93a52d3a7
workflow-type: tm+mt
source-wordcount: 812
ht-degree: 0%

---

# Resumen de atributos

La vista [!DNL Insights] _[!UICONTROL Atributos]_ muestra una lista de atributos utilizados en campañas publicitarias para la cuenta de canal seleccionada.

{{connect-insights}}

La tabla _[!UICONTROL Attributes]_ está organizada con el nombre [!UICONTROL Attribute]. Puede alternar entre los tipos de lista usando el botón **[!UICONTROL Imágenes]** y el botón **[!UICONTROL Vídeo]**. Haga clic en el icono de configuración (cog) situado encima de la parte derecha de la tabla para alternar las columnas visibles.

![Filtro y tabla de atributos](/help/assets/insights-attributes-filter.png){zoomable="yes"}

{{filter-table}}

## Detalles del atributo

Los atributos ayudan a identificar [anuncios](published-experiences.md#ad-details) y [medios](media.md#media-details) por sus detalles inherentes, como color, composición, elementos visuales y otras propiedades.

En la vista de detalles del atributo, puede ver qué anuncios utilizan el atributo seleccionado. Los detalles incluyen el rendimiento total de los atributos y un desglose de las métricas de rendimiento relacionadas con cada anuncio.

![Métricas de rendimiento de atributos](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing detecta determinadas funciones y aplica el atributo adecuado al contenido de los medios o al anuncio como etiqueta. Consulte [Categorías](#categories) para ver ejemplos de estas etiquetas. Para ver todos los atributos asociados con un anuncio, haga clic en el icono de configuración (cog) situado encima de la parte derecha de la tabla para seleccionar la columna **[!UICONTROL Attributes]**.

## Categorías

Un atributo _category_ es un grupo de clasificación que organiza atributos relacionados que comparten una característica común. Estas categorías ayudan a optimizar el descubrimiento, la identificación y la comprensión de atributos específicos al proporcionar un mayor contexto y facilitar su aplicación y uso.

GenStudio for Performance Marketing usa la IA y las capacidades de aprendizaje automático de Adobe para estudiar [imágenes](image-features.md), [vídeos](video-features.md) y [texto](text-features.md), y para aplicar atributos a anuncios y medios según la probabilidad de que sean correctos.

La lista de atributos detectados para el contenido de anuncios y medios no es exhaustiva. El contenido que contiene un completo conjunto de funciones puede limitarse a las tres funciones más dominantes identificadas por la API. Por ejemplo, la siguiente ilustración contiene varios atributos de imagen detectados, incluidos varios objetos, colores de primer plano y de fondo:

![atributos de imagen](/help/assets/category/asset-attributes.png "La imagen de Toucan incluye varios atributos detectados"){width="300" zoomable="yes"}

>[!INFO]
>
No se pueden editar las etiquetas que se detectan y aplican automáticamente.

## Rendimiento de atributos

Las métricas de perspectivas pueden ayudarle a evaluar qué atributos inspiran una mayor participación del cliente.

La siguiente tabla proporciona definiciones y perspectivas para métricas clave de marketing digital en la vista de tabla de [!UICONTROL Atributos]. Cada métrica incluye una breve definición en relación con los atributos, cómo se calcula la métrica y una o más perspectivas para ayudar a comprender su importancia e impacto en una campaña publicitaria.

| Métrica | Definición | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Atributo]** | El nombre del atributo. | Ordene la tabla haciendo clic en el encabezado de la columna de cualquiera de las métricas clave. |
| **[!UICONTROL Category]** | [category](#categories) que representa la calidad inherente de un atributo. |  |
| **[!UICONTROL # de imágenes]** | El número de imágenes que tienen este atributo. | El recuento de la tabla Atributos puede ser diferente al recuento de la vista Detalles del atributo. Esta discrepancia puede producirse si el origen del canal, como Meta y GenStudio, utiliza cálculos de resumen ligeramente diferentes. |
| **[!UICONTROL # de vídeos]** | El número de vídeos que tienen este atributo. | El recuento de la tabla Atributos puede ser diferente al recuento de la vista Detalles del atributo. Esta discrepancia puede producirse si el origen del canal, como Meta y GenStudio, utiliza cálculos de resumen ligeramente diferentes. |
| **[!UICONTROL Impresiones]** | Un recuento de cada vez que una imagen o vídeos con este atributo se cargan en el canal, independientemente de la interacción o visualización. | Un recuento alto de impresiones puede indicar una visibilidad amplia, pero si se trata de un insight de verdadero rendimiento, considéralo en relación con otras métricas de participación. |
| **[!UICONTROL Clics]** | La cantidad de veces que los usuarios interactúan con una imagen o un vídeo con este atributo. | Un alto número de clics indica un fuerte interés y participación en el contenido, que puede ser eficaz y llegar a la audiencia adecuada. |
| **[!UICONTROL tasa de pulsaciones ]**<br>_CTR_ | Porcentaje (%) de impresiones que generaron clics en imágenes o vídeos con este atributo.<br>**Cálculo**: `clicks` dividido entre `impressions` | Una alta tasa de clics indica que el contenido es muy relevante y motivador para la audiencia en cuanto a mensajería y diseño, y que se dirige de manera efectiva a los intereses de la audiencia. |
| **[!UICONTROL CPM ]**<br>_Costo por mil_ | Costo por cada mil impresiones de publicidad de una imagen o vídeo con este atributo.<br>**Cálculo**: importe total `spent` dividido por alcance y luego multiplicado por 1000 | Un valor bajo puede indicar una visibilidad rentable, especialmente cuando se asocia con una tasa de pulsaciones alta. |
| **[!UICONTROL CPA ]**<br>_Costo por acción_ | Costo promedio empleado para lograr una acción específica del cliente, como una compra o suscripción.<br>**Cálculo**: cantidad total `spent` dividida por el número de acciones del cliente completadas | Ayuda a identificar atributos que resultan en acciones valiosas del cliente. |
| **[!UICONTROL CPC ]**<br>_Costo por clic_ | Costo promedio asociado con cada clic en imágenes o vídeos con este atributo.<br>**Cálculo**: importe total `spent` dividido entre `clicks` | Unos costes medios menores pueden indicar un gasto publicitario rentable, especialmente en comparación con un aumento de las conversiones. |
| **[!UICONTROL Gasto]** | El importe gastado del presupuesto en relación con los atributos durante un período de tiempo determinado. | Un gasto elevado en un período corto puede indicar un uso rápido, lo que podría dar lugar a un agotamiento prematuro de los recursos. Realice un seguimiento de la cantidad gastada con respecto a las métricas de rendimiento clave para ayudar a monitorizar la rentabilidad general de la inversión. |
