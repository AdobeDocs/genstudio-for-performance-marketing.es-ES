---
title: Información general de Assets
description: Obtenga información sobre cómo evaluar el rendimiento de los recursos en Adobe GenStudio for Performance Marketing.
feature: Insights, Assets
exl-id: 1e93422b-2645-4e29-a216-fc1008afbfc7
source-git-commit: 4284026bf14d58eecb547d80b4bdae6ac0422078
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# Información general de Assets

La vista [!DNL Insights] _[!UICONTROL Assets]_ muestra una lista de recursos utilizados en experiencias y campañas de publicidad para la cuenta de canal seleccionada.

{{connect-insights}}

La tabla _[!UICONTROL Assets]_ está organizada con [!UICONTROL ID de recurso]. Puede alternar entre las vistas mediante el icono de lista de vistas (tabla) y el icono de vista de galería (cuadrícula). Haga clic en el icono de configuración (cog) situado encima de la parte derecha de la tabla para alternar las columnas visibles. El icono de filtro (canal) situado encima de la parte izquierda de la tabla abre el menú **[!UICONTROL Filtro]**, en el que puede seleccionar entre varias listas. Haga clic en **Restablecer** para borrar todas las selecciones de filtros.

![Filtro y tabla de Assets](/help/assets/insights-assets-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

La vista de galería de _[!UICONTROL Assets]_ muestra un collage de vistas previas de recursos y una métrica, como la tasa de pulsaciones. Haga clic en el icono de configuración (cog) situado encima de la parte derecha de la galería para abrir **[!UICONTROL Configuración de la tarjeta]** y alternar una de las tres métricas visibles:

- CPA (coste por acción)
- CTR (tasa de pulsaciones)
- CPC (coste por clic)
- Gasto

## Detalles del recurso

Un _recurso_ es una imagen, un vídeo, un texto u otro contenido creativo aprobado para su uso en iniciativas de marketing.

En la vista de detalles del recurso, puede ver qué experiencias utilizan el recurso seleccionado. Los detalles incluyen el rendimiento total del recurso, los atributos definidos por el usuario y las funciones detectadas por IA asociadas al recurso.

![Detalles del recurso](/help/assets/insights-asset-details.png){zoomable="yes"}

## Rendimiento de recursos

Las métricas de perspectivas pueden ayudarle a evaluar qué recursos contribuyen al éxito de una campaña y qué atributos de recursos son los más efectivos.

La siguiente tabla proporciona definiciones y perspectivas para métricas clave de marketing digital en la vista de tabla de [!UICONTROL Assets]. Cada métrica incluye una breve definición en relación con un recurso, cómo se calcula la métrica y una o más perspectivas para ayudar a comprender su importancia e impacto en un recurso.

| Métrica | Definición | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL ID de recurso]** | El nombre asociado con este recurso. | Ordene la tabla haciendo clic en el encabezado de la columna de cualquiera de las métricas clave. |
| **[!UICONTROL Impresiones]** | Un recuento de cada vez que el recurso se carga en el canal, independientemente de la interacción o la visualización. | Un recuento alto de impresiones puede indicar una visibilidad amplia, pero para obtener una verdadera perspectiva de rendimiento, considérala en relación con otras métricas de participación. |
| **[!UICONTROL Clics]** | La cantidad de veces que los usuarios interactúan con un elemento en el que se puede hacer clic, como un vínculo, en el recurso. | Un alto número de clics indica un fuerte interés y participación en el contenido, que puede ser eficaz y llegar a la audiencia adecuada. |
| **[!UICONTROL tasa de pulsaciones ]**<br>_CTR_ | Porcentaje (%) de impresiones que generaron clics en recursos dentro de una experiencia.<br>**Cálculo**: `clicks` dividido por `impressions` | Una alta tasa de clics indica que el contenido es muy relevante y atractivo para la audiencia. Sugiere que la mensajería y el diseño están capturando efectivamente el interés de la audiencia y motivándolos a tomar medidas. Además, un CTR alto puede implicar que el recurso está bien dirigido y resuena con la audiencia deseada, lo que conduce a un mejor rendimiento general de la campaña. |
| **[!UICONTROL CPM ]**<br>_Costo por mil_ | Coste por cada mil impresiones de publicidad del recurso.<br>**Cálculo**: importe total `spent` dividido por alcance y luego multiplicado por 1000 | Un valor bajo puede indicar una visibilidad rentable, especialmente cuando se asocia con una tasa de pulsaciones alta. |
| **[!UICONTROL CPA ]**<br>_Costo por acción_ | Coste promedio empleado para lograr una acción específica del cliente, como una compra o suscripción.<br>**Cálculo**: importe total `spent` dividido por el número de acciones del cliente completadas | Ayuda a identificar los recursos que generan valiosas acciones del cliente. |
| **[!UICONTROL CPC ]**<br>_Costo por clic_ | Coste medio asociado con cada clic en un recurso.<br>**Cálculo**: importe total `spent` dividido entre `clicks` | Unos costes medios menores pueden indicar un gasto publicitario rentable, especialmente en comparación con un aumento de las conversiones. |
| **[!UICONTROL Gasto]** | La cantidad gastada del presupuesto en relación con los activos individuales durante un período de tiempo determinado. | Un gasto elevado en un período corto puede indicar un uso rápido, lo que podría dar lugar a un agotamiento prematuro de los recursos. Realice un seguimiento de la cantidad gastada con respecto a las métricas de rendimiento clave para ayudar a monitorizar la rentabilidad general de la inversión. |
| **[!UICONTROL Recuento de experiencias]** | Número de experiencias que utilizan este recurso. | |
| **[!UICONTROL Atributos]** | Lista de atributos detectados y aplicados a este recurso. | |
