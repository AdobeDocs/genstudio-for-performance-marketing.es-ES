---
title: Información general sobre anuncios y ubicación de anuncios
description: Vea una descripción general de la participación del cliente, el presupuesto y los gastos para el rendimiento de los anuncios y la colocación de anuncios en Adobe GenStudio for Performance Marketing.
feature: Ad Performance, Text Attributes, Reporting and Insights
exl-id: e3827b1a-53d0-465c-8125-15b0e298ef3a
source-git-commit: 3448392bc3f1496dafdbed2995f40bdba9c91c31
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 0%

---

# Información general sobre anuncios y ubicación de anuncios

La vista [!DNL Insights] _[!UICONTROL Anuncios]_ muestra una lista de anuncios para la cuenta de anuncio de canal conectada. Un _anuncio_ es un recurso promocional que incluye contenido visual e interactivo que se va a distribuir a una audiencia específica como parte de una campaña de marketing. Para Facebook, los anuncios son nombres de anuncios Meta.

{{connect-insights}}

La tabla _[!UICONTROL Ads]_ está organizada con [!UICONTROL Nombres de anuncios]. Haga clic en el icono de configuración (cog) situado encima de la parte derecha de la tabla para alternar las columnas visibles. El icono de filtro (canal) situado encima de la parte izquierda de la tabla abre el menú **[!UICONTROL Filtro]**, en el que puede seleccionar entre varias listas. Seleccione **[!UICONTROL Borrar todo]** sobre la tabla para eliminar todos los filtros.

![Filtro y tabla de anuncios](/help/assets/insights-ads-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## Detalles del anuncio

Seleccione un anuncio y vea las métricas de rendimiento, los atributos de texto y las ubicaciones asociadas a cada anuncio. La _[!UICONTROL página de detalles del anuncio]_ incluye métricas para el anuncio `click-through rate`, `cost per action` y `spend`: la cantidad del presupuesto que se ha gastado en el anuncio. Dado que los anuncios pueden tener varias ubicaciones, como una fuente o un banner, puede ver un desglose de las mismas métricas para cada ubicación de publicidad. Utilice las flechas izquierda y derecha debajo de **[!UICONTROL Rendimiento por ubicación de anuncio]** para recorrer las métricas de ubicación.

![Detalles de anuncios con métricas y ubicaciones de anuncios](/help/assets/insights-ad-details.png){zoomable="yes"}

### Atributos de texto

Debajo de la vista previa del anuncio hay una lista de [!UICONTROL atributos de texto] asociados con el anuncio. Cuando los recursos y los anuncios se aprueban y almacenan en [!DNL Content], GenStudio for Performance Marketing genera etiquetas en función de sus características inherentes. Consulte [Detalles multimedia](/help/user-guide/content/asset-details.md#system-metadata) para obtener detalles acerca de los metadatos del sistema.

### Ubicaciones de anuncios

En el momento en que creó una campaña con Meta ads, es posible que haya seleccionado dónde ejecutar sus anuncios en función de la campaña [objective](channels.md#objectives). Las ubicaciones de anuncios amplían el alcance de audiencia de su anuncio.

GenStudio for Performance Marketing admite formatos de anuncio, como fuentes de recursos, anuncios de vínculos y una sola imagen o vídeo. A continuación se muestra una lista de formatos de anuncios por plataforma:

| Instagram | Facebook/Meta | Messenger | Audience Network |
| ------------ | ---------------- | ------------ | ---------------- |
| Explorar<br>Explorar inicio<br>Explorar cuadrícula Inicio<br>Alimentación<br>Carretes<br>Fuente de perfiles<br>Buscar<br>Tienda<br>Historias | Exploración empresarial<br>Fuente<br>Vídeo en flujo<br>Mercado<br>Carretes<br>Superposición de carretes<br>Columna derecha<br>Resultados de búsqueda<br>Historias<br>Fuentes de vídeo<br>Anuncios en carretes de Facebook | Bandeja de entrada<br>Historias | Nativo, banner e intersticial<br>Vídeo premiado |

#### Ubicaciones no admitidas

GenStudio for Performance Marketing no admite las siguientes ubicaciones de anuncios:

- Colaborativo
- Catálogo/catálogo Advantage+
- Experiencia de instancia
- Carrusel

## Rendimiento del anuncio

Las métricas de perspectivas pueden ayudarle a evaluar qué anuncios contribuyen al éxito de una campaña y qué ubicaciones de anuncios son las más efectivas.

La siguiente tabla proporciona definiciones y perspectivas para métricas clave de marketing digital en la vista de tabla [!UICONTROL Ads]. Cada métrica incluye una breve definición en relación con los nombres de los anuncios, cómo se calcula la métrica y una o más perspectivas para ayudar a comprender su importancia e impacto en un anuncio.

| Métrica | Definición | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Nombre del anuncio]** | Una lista de anuncios para la cuenta del canal conectado. Filtre los anuncios seleccionando una campaña. | Ordene la lista de anuncios haciendo clic en cualquiera de las métricas clave. |
| **[!UICONTROL Campaña]** | Una campaña es un conjunto de anuncios diseñados para lograr un objetivo específico. | Al filtrar la tabla Anuncios por campaña, las métricas del resumen de todos los anuncios de la campaña pueden ser diferentes a la fila de resumen de la campaña en la vista [!UICONTROL Canales]. Esta discrepancia puede producirse si el origen del canal, como Meta y GenStudio, utiliza cálculos de resumen ligeramente diferentes. |
| **[!UICONTROL Ubicaciones]** | Un recuento de las [ubicaciones](#ad-placements) del anuncio, ubicaciones en las que apareció un anuncio en la campaña. | Las ubicaciones aumentan el alcance de la audiencia.<p>Los anuncios que no muestran ninguna ubicación ni ningún medio pueden indicar un [tipo de anuncio no admitido](#unsupported-placements).</p> |
| **[!UICONTROL Medios]** | El número de recursos utilizados en el anuncio o la publicidad. | El recuento de la tabla Anuncios puede ser diferente al recuento de la vista Detalles de anuncio. Esta discrepancia puede producirse si el origen del canal, como Meta y GenStudio, utiliza cálculos de resumen ligeramente diferentes. |
| **[!UICONTROL Impresiones]** | Un recuento de cada vez que la ubicación del anuncio o el anuncio se carga en el canal, independientemente de la interacción o visualización. | Un recuento alto de impresiones puede indicar una visibilidad amplia, pero para obtener una verdadera perspectiva de rendimiento, considérala en relación con otras métricas de participación. |
| **[!UICONTROL Clics]** | El número de veces que los usuarios interactúan con un elemento en el que se puede hacer clic, como un vínculo o un botón de llamada a la acción, en una ubicación de anuncio. | Un alto número de clics indica un fuerte interés y participación en el contenido, que puede ser eficaz y llegar a la audiencia adecuada. |
| **[!UICONTROL tasa de pulsaciones ]**<br>_CTR_ | Porcentaje (%) de impresiones que generaron clics en el anuncio dentro de una campaña.<br>**Cálculo**: `clicks` dividido por `impressions` | Una alta tasa de clics indica que el contenido es muy relevante y motivador para la audiencia en cuanto a mensajería y diseño, y que se dirige de manera efectiva a los intereses de la audiencia. |
| **[!UICONTROL CPM ]**<br>_Costo por mil_ | Coste por cada mil impresiones de publicidad.<br>**Cálculo**: importe total `spent` dividido por alcance y luego multiplicado por 1000 | Un valor bajo puede indicar una visibilidad rentable, especialmente cuando se asocia con una tasa de pulsaciones alta. |
| **[!UICONTROL CPA ]**<br>_Costo por acción_ | Coste promedio empleado para lograr una acción específica del cliente, como una compra o suscripción.<br>**Cálculo**: importe total `spent` dividido por el número de acciones del cliente completadas | Se utiliza para monitorizar el gasto en anuncios que resultan en valiosas acciones de los clientes. |
| **[!UICONTROL CPC ]**<br>_Costo por clic_ | Coste medio asociado con cada clic en una ubicación de anuncio.<br>**Cálculo**: importe total `spent` dividido entre `clicks` | Unos costes medios menores pueden indicar un gasto publicitario rentable, especialmente en comparación con un aumento de las conversiones. |
| **[!UICONTROL Gasto]** | Cantidad gastada del presupuesto de Campaign durante un período de tiempo determinado para publicar este anuncio. | Un gasto elevado en un período corto puede indicar un uso rápido, lo que podría dar lugar a un agotamiento prematuro de los recursos. Realice un seguimiento de la cantidad gastada con respecto a las métricas de rendimiento clave para ayudar a monitorizar la rentabilidad general de la inversión. |

## Rendimiento de ubicación

En la vista _[!UICONTROL Página de detalles del anuncio]_, las tres métricas principales reflejan el rendimiento general del anuncio seleccionado. Sin embargo, la sección _Rendimiento por ubicación_ muestra las métricas detalladas para cada ubicación de anuncio. Utilice las flechas derecha e izquierda para desplazarse por las distintas ubicaciones de anuncios.

La siguiente tabla proporciona definiciones para métricas de rendimiento de ubicación de anuncios:

| Métrica | Definición | Insight |
| ---------------------- | ----------------------------- | ----------- |
| **[!UICONTROL tasa de pulsaciones ]**<br>_CTR_ | El porcentaje (%) de impresiones de una sola ubicación de publicidad que resultó en clics.<p>**Cálculo**:`clicks` dividido entre `impressions`<p>Esta métrica ayuda a determinar la eficacia de la colocación de anuncios para atraer a la audiencia. | Un CTR alto indica que la ubicación del anuncio es relevante y convincente para la audiencia, lo que conduce a más interacciones. |
| **[!UICONTROL CPA ]**<br>_Costo por acción_ | Coste promedio empleado en una sola ubicación de publicidad para lograr una acción del cliente deseada, como una compra o suscripción.<p>**Cálculo**: importe total `spent` dividido por el número de acciones del cliente completadas<p>Esta métrica ayuda a evaluar la rentabilidad de la colocación de anuncios a la hora de impulsar acciones valiosas. | Un CPA menor sugiere que la ubicación del anuncio es eficaz para convertir las interacciones de audiencia en acciones deseadas a un coste más bajo. |
| **[!UICONTROL CPC ]**<br>_Costo por clic_ | El coste medio asociado a cada clic en una sola ubicación de publicidad.<p>**Cálculo**: importe total `spent` dividido entre `clicks`<p>Esta métrica ayuda a evaluar la rentabilidad de la ubicación del anuncio en la generación de clics. | Un CPC más bajo indica que la colocación de anuncios está generando clics a un coste más bajo, lo que puede ser beneficioso para maximizar el retorno de la inversión. |
| **[!UICONTROL Gasto]** | La cantidad gastada en una sola ubicación de publicidad, que representa una fracción de la cantidad total gastada en todo el anuncio. Esta métrica ayuda a realizar un seguimiento de la asignación del presupuesto y la eficiencia de gasto de cada ubicación de publicidad. | La supervisión del gasto puede ayudar a garantizar que los recursos se utilicen de forma eficaz en diferentes ubicaciones. |
