---
title: Información general de medios
description: Obtenga información sobre cómo evaluar el rendimiento de los medios en Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Media Performance, Content Attributes
exl-id: 1e93422b-2645-4e29-a216-fc1008afbfc7
TQID: https://experienceleague.adobe.com/fSBgN1uvr39dd7AV3Kvr3D5UnSDY2-dE1aX1g2Q7fTc
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f321b88b-6bb7-49cc-a16a-ae2b665ebd32
subfeature_v2:
  - id: a29f532b-105a-4aec-8a5d-e7e725214866
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
  - id: dd48f9df-f2e2-49fe-a918-332a8e240ffe
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 647
ht-degree: 0%

---

# Resumen de medios

La vista [!DNL Insights] _[!UICONTROL Medios]_ muestra una lista de medios utilizados en anuncios y campañas de publicidad para la cuenta seleccionada. _Medios_ representa una imagen, un vídeo, un texto u otro contenido creativo aprobado para su uso en iniciativas de marketing.

{{connect-insights}}

La tabla _[!UICONTROL Media]_ está organizada con **[!UICONTROL Media ID]**. Puede alternar entre las vistas mediante el icono de lista de vistas (tabla) y el icono de vista de galería (cuadrícula). Haga clic en el icono de configuración (cog) situado encima de la parte derecha de la tabla para alternar las columnas visibles.

![Filtro y tabla de medios](/help/assets/insights-media-filter.png){zoomable="yes"}

La vista de galería _[!UICONTROL Media]_ muestra un collage de vistas previas de medios y una métrica, como la tasa de pulsaciones. Haga clic en el icono de configuración (cog) situado encima de la parte derecha de la galería para abrir **[!UICONTROL Configuración de la tarjeta]** y alternar una de las tres métricas visibles:

- CPA (coste por acción)
- CTR (tasa de pulsaciones)
- CPC (coste por clic)
- Gasto

{{filter-table}}

## Detalles multimedia

En la vista _Detalles multimedia_, puede ver qué anuncios utilizan los medios seleccionados. Los detalles incluyen el rendimiento total de los medios, los anuncios que utilizan los medios, los atributos definidos por el usuario y las funciones detectadas por IA asociadas con los medios.

![Detalles multimedia](/help/assets/insights-media-details.png){zoomable="yes"}

### Atributos de medios

{{$include /help/_includes/generated-attributes.md}}

## Rendimiento de medios

Las métricas de perspectivas pueden ayudarle a evaluar qué medios contribuyen al éxito de una campaña y qué atributos de medios son los más efectivos.

La siguiente tabla proporciona definiciones y perspectivas para métricas clave de marketing digital en la vista de tabla de [!UICONTROL Media]. Cada métrica incluye una breve definición en relación con los medios, cómo se calcula la métrica y una o más perspectivas para ayudar a comprender su importancia e impacto.

| Métrica | Definición | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL ID de medio]** | El nombre asociado a una imagen, vídeo, texto u otro contenido creativo. | Ordene la tabla haciendo clic en el encabezado de la columna de cualquiera de las métricas clave. |
| **[!UICONTROL Impresiones]** | Recuento de cada vez que los medios se cargan en el canal, independientemente de la interacción o la visualización. | Un recuento alto de impresiones puede indicar una visibilidad amplia, pero si se trata de un insight de verdadero rendimiento, considéralo en relación con otras métricas de participación. |
| **[!UICONTROL Clics]** | El número de veces que los usuarios interactúan con un elemento en el que se puede hacer clic, como un vínculo, en los medios. | Un alto número de clics indica un fuerte interés y participación en el contenido, que puede ser eficaz y llegar a la audiencia adecuada. |
| **[!UICONTROL tasa de pulsaciones &#x200B;]**<br>_CTR_ | Porcentaje (%) de impresiones que generaron clics en medios dentro de un anuncio.<br>**Cálculo**: `clicks` dividido entre `impressions` | Una alta tasa de clics indica que el contenido es muy relevante y atractivo para la audiencia. Sugiere que la mensajería y el diseño están capturando efectivamente el interés de la audiencia y motivándolos a tomar medidas. Además, un CTR alto puede implicar que los medios están bien dirigidos y resuenan con la audiencia deseada, lo que conduce a un mejor rendimiento general de la campaña. |
| **[!UICONTROL CPM &#x200B;]**<br>_Costo por mil_ | Costo promedio por cada mil impresiones multimedia.<br>**Cálculo**: importe total `spent` dividido por el número de impresiones y multiplicado por 1000 | Un valor de CPM bajo puede indicar un rendimiento de medios rentable, especialmente cuando se combina con una tasa de pulsaciones alta. |
| **[!UICONTROL CPA &#x200B;]**<br>_Costo por acción_ | Costo promedio empleado para lograr una acción específica del cliente, como una compra o suscripción.<br>**Cálculo**: cantidad total `spent` dividida por el número de acciones del cliente completadas | Ayuda a identificar medios que generan valiosas acciones para los clientes. |
| **[!UICONTROL CPC &#x200B;]**<br>_Costo por clic_ | Costo promedio asociado con cada clic en el medio.<br>**Cálculo**: importe total `spent` dividido entre `clicks` | Unos costes medios menores pueden indicar un gasto publicitario rentable, especialmente en comparación con un aumento de las conversiones. |
| **[!UICONTROL Gasto]** | La cantidad gastada del presupuesto en relación con los medios individuales durante un período de tiempo determinado. | Un gasto elevado en un período corto puede indicar un uso rápido, lo que podría dar lugar a un agotamiento prematuro de los recursos. Realice un seguimiento de la cantidad gastada con respecto a las métricas de rendimiento clave para ayudar a monitorizar la rentabilidad general de la inversión. |
| **[!UICONTROL Se usa en estos anuncios]** | El número de anuncios que utilizan este medio. | |
| **Atributos** | Lista de características inherentes presentes en este medio. | Los atributos ayudan a identificar los elementos creativos que más interesan a su audiencia. |
