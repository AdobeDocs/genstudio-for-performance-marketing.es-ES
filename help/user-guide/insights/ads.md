---
title: Información general sobre anuncios y ubicación de anuncios
description: Vea una descripción general de la participación del cliente, el presupuesto y los gastos para el rendimiento de los anuncios y la colocación de anuncios en Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Ad Performance, Text Attributes, Reporting and Insights
exl-id: e3827b1a-53d0-465c-8125-15b0e298ef3a
source-git-commit: e053c91ebb40a9625ce22281a89feaa9cccab956
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 0%

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

{{empty-table}}

## Filtrar anuncios

El icono de filtro (canal) situado encima de la parte izquierda abre el menú **[!UICONTROL Filtro]**, en el que puede seleccionar entre varias listas. Con algunos filtros, puede aprovechar palabras clave precisas para restringir la lista de criterios. Los filtros de palabras clave son especialmente útiles para campañas que siguen una convención de nombres compleja con varios identificadores únicos, como los siguientes:

- Código o nombre de región específico: `NA`, `EMEA`
- Acrónimos de tipo de contenido: `EB`, `CHT` o `DSP`
- Códigos de ofertas o siglas: `OFFER2023`, `PROMO`

**Para filtrar por campañas**:

1. Expanda el filtro **[!UICONTROL Campaigns]** y haga clic en **[!UICONTROL Select]**.
1. En el campo de búsqueda, introduzca palabras clave separadas por comas.

   Utilice tantas palabras clave como sea necesario para restringir la lista:

   ![Seleccionar campañas](/help/assets/insights-select-campaign.png){width=400}

1. Seleccione una o más campañas de la búsqueda resultante y haga clic en **[!UICONTROL Aplicar]**.

   Las campañas seleccionadas aparecerán ahora en la lista _[!UICONTROL Filtrar por]_ situada encima de la tabla o galería de anuncios, lo que le permite centrarse en los anuncios asociados con las campañas seleccionadas.

>[!NOTE]
>
>El filtro aplicado persiste en todas las vistas de [!DNL Insights]. Seleccione **[!UICONTROL Borrar todo]** sobre la tabla o galería de anuncios para eliminar todos los filtros seleccionados.

### Descargar resultados de tabla

{{$include /help/_includes/download-insights.md}}

## Detalles del anuncio

Seleccione un anuncio y vea las métricas de rendimiento, los atributos de texto y las ubicaciones asociadas a cada anuncio. La _[!UICONTROL página de detalles del anuncio]_ incluye métricas para el anuncio `click-through rate`, `cost per action` y `spend`: la cantidad del presupuesto que se ha gastado en el anuncio. Dado que los anuncios pueden tener varias ubicaciones, como una fuente o un banner, puede ver un desglose de las mismas métricas para cada ubicación de publicidad. Utilice las flechas izquierda y derecha debajo de **[!UICONTROL Rendimiento por ubicación de anuncio]** para recorrer las métricas de ubicación.

![Detalles de anuncios con métricas y ubicaciones de anuncios](/help/assets/insights-ad-details.png){zoomable="yes"}

### Atributos de anuncio

Debajo de la vista previa del anuncio hay una lista de atributos asociados con el anuncio.

{{$include /help/_includes/generated-attributes.md}}

### Formatos de anuncio

Los formatos de anuncio hacen referencia a los distintos elementos creativos y diseños que se utilizan para alinearse con los objetivos de la campaña, atraer a la audiencia de destino y ayudar a rastrear las métricas de rendimiento.

[!DNL Insights] en GenStudio for Performance Marketing admite actualmente los siguientes formatos de publicidad disponibles.

| Compatible | No compatible |
|-----------|-------------|
| Especificación de fuente de recursos (optimización de ubicación)<br>Imagen o vídeo únicos<br>Vínculo | Carrusel<br>Catálogo<br>Colaborativo<br>Experiencia instantánea<br>Especificaciones de la fuente de recursos (además de la optimización de la ubicación)<br>Llamada (imagen y vídeo)<br>Aplicación (imagen y vídeo)<br>Mensajería<br>Posible cliente (imagen y vídeo)<br>Presentación de diapositivas (vídeo)<br>Colección (imagen y recurso de vídeo a pantalla completa)<br>Tienda (imagen y vídeo)<br>Foto o vídeo de la publicación de la página, publicación de Instagram<br>Contenido de marca<br>Catálogo flexible<br>Advantage+ |

### Ubicaciones de anuncios

Las ubicaciones de los anuncios hacen referencia a las ubicaciones o plataformas específicas en las que los anuncios aparecen dentro de una campaña. Estas ubicaciones determinan cómo y dónde interactúa la audiencia con el contenido. Las ubicaciones de anuncios amplían el alcance de la audiencia, lo que ayuda a maximizar la visibilidad, la participación y la eficacia general de la campaña.

Al crear una campaña con Meta ads, es posible que hayas seleccionado dónde publicar tus anuncios según la campaña [objective](channels.md#objectives).

A continuación se muestra una lista de ubicaciones de anuncios compatibles:

| Audience Network | Facebook/Meta \* | Instagram | Messenger |
|--------------------|--------------------|-------------------------|---------------------|
| Vídeo premiado | Fuente<br>Fuentes de vídeo<br>Historias<br>Mercado<br>Columna derecha<br>Carretes<br>Superposición de carretes<br>Vídeo en el flujo<br>Buscar<br>Fuente de discoteca para empresas<br>Fuente de perfiles | Historias<br>Fuente<br>Explorar<br>Carretes<br>Explorar la cuadrícula Inicio<br>Fuente de perfiles<br>Buscar<br>Secuencia | Historias<br>Bandeja de entrada |

\* Vea [Acerca de las ubicaciones de los anuncios en las metatecnologías](https://www.facebook.com/business/help/407108559393196?id=369787570424415) en el _Centro de ayuda para metanegocios_.

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
| **[!UICONTROL tasa de pulsaciones &#x200B;]**<br>_CTR_ | Porcentaje (%) de impresiones que generaron clics en el anuncio dentro de una campaña.<br>**Cálculo**: `clicks` dividido por `impressions` | Una alta tasa de clics indica que el contenido es muy relevante y motivador para la audiencia en cuanto a mensajería y diseño, y que se dirige de manera efectiva a los intereses de la audiencia. |
| **[!UICONTROL CPM &#x200B;]**<br>_Costo por mil_ | El coste medio por cada mil impresiones de publicidad.<br>**Cálculo**: importe total `spent` dividido por alcance y luego multiplicado por 1000 | Un valor bajo puede indicar una visibilidad rentable, especialmente cuando se asocia con una tasa de pulsaciones alta. |
| **[!UICONTROL CPA &#x200B;]**<br>_Costo por acción_ | Coste promedio empleado para realizar una acción específica del cliente, como una compra o suscripción.<br>**Cálculo**: importe total `spent` dividido por el número de acciones del cliente completadas | Se utiliza para monitorizar el gasto en anuncios que resultan en valiosas acciones de los clientes. |
| **[!UICONTROL CPC &#x200B;]**<br>_Costo por clic_ | El coste medio asociado con cada clic en una ubicación de anuncio.<br>**Cálculo**: importe total `spent` dividido entre `clicks` | Unos costes medios menores pueden indicar un gasto publicitario rentable, especialmente en comparación con un aumento de las conversiones. |
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
