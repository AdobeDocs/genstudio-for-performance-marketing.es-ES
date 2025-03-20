---
title: Resumen de medios
description: Obtenga información sobre cómo evaluar el rendimiento de los medios en Adobe GenStudio for Performance Marketing.
feature: Reporting and Insights, Media Performance, Content Attributes
exl-id: 1e93422b-2645-4e29-a216-fc1008afbfc7
source-git-commit: 3448392bc3f1496dafdbed2995f40bdba9c91c31
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 0%

---

# Resumen de medios

La vista [!DNL Insights] _[!UICONTROL Medios]_ muestra una lista de medios utilizados en anuncios y campañas de publicidad para la cuenta seleccionada. _Medios_ representa una imagen, un vídeo, un texto u otro contenido creativo aprobado para su uso en iniciativas de marketing.

{{connect-insights}}

La tabla _[!UICONTROL Media]_ está organizada con **[!UICONTROL Media ID]**. Puede alternar entre las vistas mediante el icono de lista de vistas (tabla) y el icono de vista de galería (cuadrícula). Haga clic en el icono de configuración (cog) situado encima de la parte derecha de la tabla para alternar las columnas visibles. El icono de filtro (canal) situado encima de la parte izquierda de la tabla abre el menú **[!UICONTROL Filtro]**, en el que puede seleccionar entre varias listas. Seleccione **[!UICONTROL Borrar todo]** sobre la tabla para eliminar todos los filtros.

![Filtro y tabla de medios](/help/assets/insights-media-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

La vista de galería _[!UICONTROL Media]_ muestra un collage de vistas previas de medios y una métrica, como la tasa de pulsaciones. Haga clic en el icono de configuración (cog) situado encima de la parte derecha de la galería para abrir **[!UICONTROL Configuración de la tarjeta]** y alternar una de las tres métricas visibles:

- CPA (coste por acción)
- CTR (tasa de pulsaciones)
- CPC (coste por clic)
- Gasto

## Detalles multimedia

En la vista _Detalles multimedia_, puede ver qué anuncios utilizan los medios seleccionados. Los detalles incluyen el rendimiento total de los medios, los anuncios que utilizan los medios, los atributos definidos por el usuario y las funciones detectadas por IA asociadas con los medios.

![Detalles multimedia](/help/assets/insights-media-details.png){zoomable="yes"}

## Rendimiento de medios

Las métricas de perspectivas pueden ayudarle a evaluar qué medios contribuyen al éxito de una campaña y qué atributos de medios son los más efectivos.

La siguiente tabla proporciona definiciones y perspectivas para métricas clave de marketing digital en la vista de tabla de [!UICONTROL Media]. Cada métrica incluye una breve definición en relación con los medios, cómo se calcula la métrica y una o más perspectivas para ayudar a comprender su importancia e impacto.

| Métrica | Definición | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL ID de medio]** | El nombre asociado a una imagen, vídeo, texto u otro contenido creativo. | Ordene la tabla haciendo clic en el encabezado de la columna de cualquiera de las métricas clave. |
| **[!UICONTROL Impresiones]** | Recuento de cada vez que los medios se cargan en el canal, independientemente de la interacción o la visualización. | Un recuento alto de impresiones puede indicar una visibilidad amplia, pero para obtener una verdadera perspectiva de rendimiento, considérala en relación con otras métricas de participación. |
| **[!UICONTROL Clics]** | El número de veces que los usuarios interactúan con un elemento en el que se puede hacer clic, como un vínculo, en los medios. | Un alto número de clics indica un fuerte interés y participación en el contenido, que puede ser eficaz y llegar a la audiencia adecuada. |
| **[!UICONTROL tasa de pulsaciones ]**<br>_CTR_ | Porcentaje (%) de impresiones que generaron clics en medios dentro de un anuncio.<br>**Cálculo**: `clicks` dividido por `impressions` | Una alta tasa de clics indica que el contenido es muy relevante y atractivo para la audiencia. Sugiere que la mensajería y el diseño están capturando efectivamente el interés de la audiencia y motivándolos a tomar medidas. Además, un CTR alto puede implicar que los medios están bien dirigidos y resuenan con la audiencia deseada, lo que conduce a un mejor rendimiento general de la campaña. |
| **[!UICONTROL CPM ]**<br>_Costo por mil_ | Coste por cada mil impresiones en los medios.<br>**Cálculo**: importe total `spent` dividido por el número de impresiones y luego multiplicado por 1000 | Un valor de CPM bajo puede indicar un rendimiento de medios rentable, especialmente cuando se combina con una tasa de pulsaciones alta. |
| **[!UICONTROL CPA ]**<br>_Costo por acción_ | Coste promedio empleado para lograr una acción específica del cliente, como una compra o suscripción.<br>**Cálculo**: importe total `spent` dividido por el número de acciones del cliente completadas | Ayuda a identificar medios que generan valiosas acciones para los clientes. |
| **[!UICONTROL CPC ]**<br>_Costo por clic_ | Coste medio asociado con cada clic en el contenido.<br>**Cálculo**: importe total `spent` dividido entre `clicks` | Unos costes medios menores pueden indicar un gasto publicitario rentable, especialmente en comparación con un aumento de las conversiones. |
| **[!UICONTROL Gasto]** | La cantidad gastada del presupuesto en relación con los medios individuales durante un período de tiempo determinado. | Un gasto elevado en un período corto puede indicar un uso rápido, lo que podría dar lugar a un agotamiento prematuro de los recursos. Realice un seguimiento de la cantidad gastada con respecto a las métricas de rendimiento clave para ayudar a monitorizar la rentabilidad general de la inversión. |
| **[!UICONTROL Se usa en estos anuncios]** | El número de anuncios que utilizan este medio. | |
| **[!UICONTROL Atributos]** | Lista de atributos detectados y aplicados a este medio. | |
