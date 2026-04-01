---
title: Información general sobre anuncios y ubicación de anuncios
description: Vea una descripción general de la participación del cliente, el presupuesto y los gastos para el rendimiento de los anuncios y la colocación de anuncios en Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Ad Performance, Text Attributes, Reporting and Insights
exl-id: e3827b1a-53d0-465c-8125-15b0e298ef3a
TQID: https://experienceleague.adobe.com/TVvHSbmD8vvc4y9xmg4iPnT-eWKwjln5730LUdgUW0k
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
  - id: bb0d2eba-617d-4fdd-b920-2f535b5c031c
  - id: dd48f9df-f2e2-49fe-a918-332a8e240ffe
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: b5520579-b31f-4df7-9281-f0d9f91e2edc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 59f51bf35c5ad81845d2cd11c6659a0833e4de7b
workflow-type: tm+mt
source-wordcount: 1457
ht-degree: 1%

---

# Información general sobre anuncios y ubicación de anuncios

La vista [!DNL Insights] _[!UICONTROL Anuncios]_ muestra una lista de anuncios para la cuenta de anuncio de canal conectada. Un _anuncio_ es un recurso promocional que incluye contenido visual e interactivo que se va a distribuir a una audiencia específica como parte de una campaña de marketing.

{{connect-insights}}

La tabla _[!UICONTROL Ads]_ está organizada con [!UICONTROL Nombres de anuncios]. Haga clic en el icono de configuración (cog) situado encima de la parte derecha de la tabla para alternar las columnas visibles.

![Filtro y tabla de anuncios](/help/assets/insights-ads-filter.png){zoomable="yes"}

La vista de galería _[!UICONTROL Ad]_ muestra un collage de vistas previas de anuncios y una métrica, como la tasa de pulsaciones. Haga clic en el icono de configuración (cog) situado encima de la parte derecha de la galería para abrir **[!UICONTROL Configuración de la tarjeta]** y alternar una de las tres métricas visibles:

- CPA (coste por acción)
- CTR (tasa de pulsaciones)
- CPC (coste por clic)
- Gasto

{{filter-table}}

## Detalles del anuncio

Seleccione un anuncio y vea las métricas de rendimiento, los atributos de texto y las ubicaciones asociadas a cada anuncio. La _[!UICONTROL página de detalles del anuncio]_ incluye métricas para el anuncio `click-through rate`, `cost per action` y `spend`: la cantidad del presupuesto que se ha gastado en el anuncio. Dado que los anuncios pueden tener varias ubicaciones, como una fuente o un banner, puede ver un desglose de las mismas métricas para cada ubicación de publicidad. Utilice las flechas izquierda y derecha debajo de **[!UICONTROL Rendimiento por ubicación de anuncio]** para recorrer las métricas de ubicación.

![Detalles de anuncios con métricas y ubicaciones de anuncios](/help/assets/insights-ad-details.png){zoomable="yes"}

### Atributos de anuncio

Debajo de la vista previa del anuncio hay una lista de atributos asociados con el anuncio.

{{$include /help/_includes/generated-attributes.md}}

### Formatos de anuncio

Los formatos de anuncio hacen referencia a los distintos elementos creativos y diseños que se utilizan para alinearse con los objetivos de la campaña, atraer a la audiencia de destino y ayudar a rastrear las métricas de rendimiento.

[!DNL Insights] en GenStudio for Performance Marketing admite actualmente los siguientes formatos de publicidad disponibles.

| Canal | Compatible | No compatible |
|---|---|---|
| Meta | <ul><li>Anuncios dinámicos</li><li>Anuncios de vínculos</li><li>Anuncios de imagen simples</li><li>Anuncios de vídeo simples</li><li>Anuncios de tienda</li></ul> | <ul><li>Ventaja + Anuncios de catálogo</li><li>Anuncios de carrusel</li><li>Anuncios de Messenger</li><li>Anuncios de posibles clientes</li><li>Anuncios de colección</li><li>Anuncios de llamadas</li><li>Anuncios de publicación de páginas en propiedad</li><li>Anuncios de asociación</li><li>Anuncios flexibles</li></ul> |
| LinkedIn | <ul><li>Anuncios de imagen única</li><li>Anuncios de vídeo único</li><li>Anuncios de artículos</li></ul> | <ul><li>Anuncios de carrusel</li><li>Anuncios de documentos</li><li>Anuncios de eventos</li><li>Thought Leader Ads</li><li>Anuncios de generación de clientes potenciales</li><li>Anuncios de seguidores</li><li>Anuncios de conversación</li><li>Anuncios destacados</li><li>Anuncios de trabajo</li><li>Anuncios de contenido</li><li>Anuncios de mensajes</li></ul> |
| TikTok | <ul><li>Anuncios de imagen única</li><li>Anuncios de vídeo único</li></ul> | <ul><li>Anuncios en el canal (vídeo, Spark, carrusel)</li><li>Anuncios Premium (TopView, Brand Takeover)</li><li>Anuncios interactivos (retos de etiquetas, efectos de marca)</li><li>Commerce Ads (Shopping, Catalog, LIVE)</li><li>Posible cliente y anuncios de mensajería</li><li>Es difícil clasificarlos, ya que no tenemos los recursos para determinar el tipo de anuncio</li></ul> |
| DV360 | <ul><li>DISPLAY_AND_VIDEO_ADS</li><li>YOUTUBE_AND_PARTNERS_AD</li></ul> | El canal de medios de pago no proporciona acceso para recuperar recursos creativos, lo que dificulta la clasificación precisa de los tipos de anuncios. |
| Innovid | N/D | Es difícil clasificarlos, ya que no tenemos los recursos para determinar el tipo de anuncio. |

### Ubicaciones de anuncios

Las ubicaciones de los anuncios hacen referencia a las ubicaciones o plataformas específicas en las que los anuncios aparecen dentro de una campaña. Estas ubicaciones determinan cómo y dónde interactúa la audiencia con el contenido. Las ubicaciones de anuncios amplían el alcance de la audiencia, lo que ayuda a maximizar la visibilidad, la participación y la eficacia general de la campaña.

Al crear una campaña, es posible que hayas seleccionado dónde publicar tus anuncios en función del [objetivo](campaigns.md#objectives) de la campaña.

A continuación se muestra una lista de las ubicaciones de anuncios compatibles con Meta:

| Audience Network | Facebook/Meta \* | Instagram | Messenger |
|--------------------|--------------------|-------------------------|---------------------|
| Vídeo premiado | Fuente<br>Fuentes de vídeo<br>Historias<br>Mercado<br>Columna derecha<br>Carretes<br>Superposición de carretes<br>Vídeo en el flujo<br>Buscar<br>Fuente de discoteca para empresas<br>Fuente de perfiles | Historias<br>Fuente<br>Explorar<br>Carretes<br>Explorar la cuadrícula Inicio<br>Fuente de perfiles<br>Buscar<br>Secuencia | Historias<br>Bandeja de entrada |

\* Consulte [Acerca de las ubicaciones de anuncios en tecnologías de Meta](https://www.facebook.com/business/help/407108559393196?id=369787570424415) en el _Centro de ayuda para empresas de Meta_.

## Rendimiento del anuncio

Las métricas de perspectivas pueden ayudarle a evaluar qué anuncios contribuyen al éxito de una campaña y qué ubicaciones de anuncios son las más efectivas.

La siguiente tabla proporciona definiciones y perspectivas para métricas clave de marketing digital en la vista de tabla [!UICONTROL Ads]. Cada métrica incluye una breve definición en relación con los nombres de los anuncios, cómo se calcula la métrica y una o más perspectivas para ayudar a comprender su importancia e impacto en un anuncio.

| Métrica | Definición | Insight |
| ---------------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Nombre del anuncio]** | Una lista de anuncios para la cuenta del canal conectado. Filtre los anuncios seleccionando una campaña. | Ordene la lista de anuncios haciendo clic en cualquiera de las métricas clave. |
| **[!UICONTROL Campaña]** | Una campaña es un conjunto de anuncios diseñados para lograr un objetivo específico. | Al filtrar la tabla Anuncios por campaña, las métricas del resumen de todos los anuncios de la campaña pueden ser diferentes a la fila de resumen de la campaña en la vista [!UICONTROL Canales]. Esta discrepancia puede producirse si el origen del canal, como Meta y GenStudio, utiliza cálculos de resumen ligeramente diferentes. |
| **[!UICONTROL Ubicaciones]** | Un recuento de las [ubicaciones](#ad-placements) del anuncio, ubicaciones en las que apareció un anuncio en la campaña. | Las ubicaciones aumentan el alcance de la audiencia.<p>Los anuncios que no muestran ninguna ubicación ni ningún medio pueden indicar un [tipo de anuncio no admitido](#unsupported-placements).</p> |
| **[!UICONTROL Medios]** | El número de recursos utilizados en las ubicaciones de anuncios y anuncios | El recuento de la tabla Anuncios puede ser diferente al recuento de la vista Detalles de anuncio. Esta discrepancia puede producirse si el origen del canal, como Meta y GenStudio, utiliza cálculos de resumen ligeramente diferentes. |
| **[!UICONTROL Impresiones]** | Un recuento de cada vez que la ubicación del anuncio o el anuncio se carga en el canal, independientemente de la interacción o visualización. | Un recuento alto de impresiones puede indicar una visibilidad amplia, pero si se trata de un insight de verdadero rendimiento, considéralo en relación con otras métricas de participación. |
| **[!UICONTROL Clics]** | El número de veces que los usuarios interactúan con un elemento en el que se puede hacer clic, como un vínculo o un botón de call-to-action, en una ubicación de anuncio. | Un alto número de clics indica un fuerte interés y participación en el contenido, que puede ser eficaz y llegar a la audiencia adecuada. |
| **[!UICONTROL tasa de pulsaciones &#x200B;]**<br>_CTR_ | Porcentaje (%) de impresiones que generaron clics en el anuncio dentro de una campaña.<br>**Cálculo**: `clicks` dividido entre `impressions` | Una alta tasa de clics indica que el contenido es muy relevante y motivador para la audiencia en cuanto a mensajería y diseño, y que se dirige de manera efectiva a los intereses de la audiencia. |
| **[!UICONTROL CPM &#x200B;]**<br>_Costo por mil_ | Costo promedio por cada mil impresiones de publicidad.<br>**Cálculo**: importe total `spent` dividido por alcance y luego multiplicado por 1000 | Un valor bajo puede indicar una visibilidad rentable, especialmente cuando se asocia con una tasa de pulsaciones alta. |
| **[!UICONTROL CPA &#x200B;]**<br>_Costo por acción_ | Costo promedio empleado para realizar una acción específica del cliente, como una compra o suscripción.<br>**Cálculo**: cantidad total `spent` dividida por el número de acciones del cliente completadas | Se utiliza para monitorizar el gasto en anuncios que resultan en valiosas acciones de los clientes. |
| **[!UICONTROL CPC &#x200B;]**<br>_Costo por clic_ | Costo promedio asociado con cada clic en una ubicación de anuncio.<br>**Cálculo**: importe total `spent` dividido entre `clicks` | Unos costes medios menores pueden indicar un gasto publicitario rentable, especialmente en comparación con un aumento de las conversiones. |
| **[!UICONTROL Gasto]** | Cantidad gastada del presupuesto de Campaign durante un período de tiempo determinado para publicar este anuncio. | Un gasto elevado en un período corto puede indicar un uso rápido, lo que podría dar lugar a un agotamiento prematuro de los recursos. Realice un seguimiento de la cantidad gastada con respecto a las métricas de rendimiento clave para ayudar a monitorizar la rentabilidad general de la inversión. |
| **Atributos** | Lista de características inherentes presentes en este anuncio. | Los atributos ayudan a identificar los elementos creativos que más interesan a su audiencia. Ver [Categorías](/help/user-guide/insights/attributes.md#categories). |

## Rendimiento de ubicación

En la vista _[!UICONTROL Página de detalles del anuncio]_, las tres métricas principales reflejan el rendimiento general del anuncio seleccionado. Sin embargo, la sección _Rendimiento por ubicación_ muestra las métricas detalladas para cada ubicación de anuncio. Utilice las flechas derecha e izquierda para desplazarse por las distintas ubicaciones de anuncios.

La siguiente tabla proporciona definiciones para métricas de rendimiento de ubicación de anuncios:

| Métrica | Definición | Insight |
| ---------------------------- | ----------------------------- | --------------------------------- |
| **[!UICONTROL tasa de pulsaciones &#x200B;]**<br>_CTR_ | El porcentaje (%) de impresiones de una sola ubicación de publicidad que resultó en clics.<p>**Cálculo**:`clicks` dividido entre `impressions`<p>Esta métrica ayuda a determinar la eficacia de la colocación de anuncios para atraer a la audiencia. | Un CTR alto indica que la ubicación del anuncio es relevante y convincente para la audiencia, lo que conduce a más interacciones. |
| **[!UICONTROL CPA &#x200B;]**<br>_Costo por acción_ | Coste promedio empleado en una sola ubicación de publicidad para lograr una acción del cliente deseada, como una compra o suscripción.<p>**Cálculo**: importe total `spent` dividido por el número de acciones del cliente completadas<p>Esta métrica ayuda a evaluar la rentabilidad de la colocación de anuncios a la hora de impulsar acciones valiosas. | Un CPA menor sugiere que la ubicación del anuncio es eficaz para convertir las interacciones de audiencia en acciones deseadas a un coste más bajo. |
| **[!UICONTROL CPC &#x200B;]**<br>_Costo por clic_ | El coste medio asociado a cada clic en una sola ubicación de publicidad.<p>**Cálculo**: importe total `spent` dividido entre `clicks`<p>Esta métrica ayuda a evaluar la rentabilidad de la ubicación del anuncio en la generación de clics. | Un CPC más bajo indica que la colocación de anuncios está generando clics a un coste más bajo, lo que puede ser beneficioso para maximizar el retorno de la inversión. |
| **[!UICONTROL Gasto]** | La cantidad gastada en una sola ubicación de publicidad, que representa una fracción de la cantidad total gastada en todo el anuncio. Esta métrica ayuda a realizar un seguimiento de la asignación del presupuesto y la eficiencia de gasto de cada ubicación de publicidad. | La supervisión del gasto puede ayudar a garantizar que los recursos se utilicen de forma eficaz en diferentes ubicaciones. |
| **Atributos** | Lista de funciones inherentes presentes en esta ubicación de anuncio. | Los atributos ayudan a identificar los elementos creativos que más interesan a su audiencia. Ver [Categorías](/help/user-guide/insights/attributes.md#categories). |
