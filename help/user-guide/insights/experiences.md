---
title: Resumen de experiencias
description: Vea una descripción general de la participación del cliente, el presupuesto y los gastos para obtener experiencias y el rendimiento de la ubicación de los anuncios en Adobe GenStudio for Performance Marketing.
feature: Insights, Experiences, Attributes
exl-id: e3827b1a-53d0-465c-8125-15b0e298ef3a
source-git-commit: 2abd2d874fb9ce515c9ec15bd6130b5a4dc8bd48
workflow-type: tm+mt
source-wordcount: '1092'
ht-degree: 0%

---

# Resumen de experiencias

La vista [!DNL Insights] _[!UICONTROL Experiencias]_ muestra una lista de experiencias para la cuenta de anuncios del canal conectado. Para Facebook, las experiencias son nombres de anuncios Meta.

{{connect-insights}}

La tabla _[!UICONTROL Experiencias]_ está organizada con [!UICONTROL nombres de anuncios]. Haga clic en el icono de configuración (cog) situado encima de la parte derecha de la tabla para alternar las columnas visibles. El icono de filtro (canal) situado encima de la parte izquierda de la tabla abre el menú **[!UICONTROL Filtro]**, en el que puede seleccionar entre las listas [!UICONTROL Cuenta] y [!UICONTROL Campaña] para filtrar los nombres de los anuncios de la tabla.

![Filtro y tabla de experiencias](/help/assets/insights-experiences-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## Detalles de la experiencia

Una _experiencia_ es un recurso promocional que incluye contenido visual e interactivo que se va a distribuir a una audiencia específica como parte de una campaña de marketing.

Seleccione una experiencia (nombre del anuncio) y vea las métricas de rendimiento, los atributos de texto y las ubicaciones asociados a cada anuncio. En la vista de detalles, puede analizar las métricas de una experiencia en función de su ubicación de publicidad y los esfuerzos de marketing realizados dentro de un intervalo de fechas especificado.

La vista de detalles incluye un anuncio general de métricas `click-through rate`, `cost per action` y `spend`, en el que se indica la cantidad del presupuesto que se ha incluido en el anuncio. Dado que los anuncios pueden tener varias ubicaciones, como una fuente o un banner, puede ver un desglose de las mismas métricas para cada ubicación de publicidad. Utilice las flechas izquierda y derecha debajo de **[!UICONTROL Rendimiento por ubicación de anuncio]** para recorrer las métricas de ubicación.

![Detalles de anuncios con métricas y ubicaciones de anuncios](/help/assets/insights-experience-details.png){zoomable="yes"}

### Atributos de texto

Debajo de la vista previa de la experiencia se encuentra una lista de [!UICONTROL Atributos de texto] asociados con el anuncio. Cuando los recursos y las experiencias se aprueban y almacenan en [!DNL Content], GenStudio for Performance Marketing genera etiquetas en función de sus características inherentes. Consulte [Detalles del recurso](../content/asset-details.md#system-metadata) para obtener detalles acerca de los metadatos del sistema.

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

## Rendimiento de experiencia

Las métricas de perspectivas pueden ayudarle a evaluar qué experiencias contribuyen al éxito de una campaña y qué ubicaciones de anuncios son las más efectivas.

La siguiente tabla proporciona definiciones y perspectivas para métricas clave de marketing digital en la vista de tabla de [!UICONTROL Experiencias]. Cada métrica incluye una breve definición en relación con los nombres de los anuncios, cómo se calcula la métrica y una o más perspectivas para ayudar a comprender su importancia e impacto en una experiencia.

| Métrica | Definición | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Nombre de experiencia]** | Una lista de experiencias para la cuenta del canal conectado. Filtre los anuncios seleccionando una campaña. | Ordene la lista de experiencias haciendo clic en cualquiera de las métricas clave. |
| **[!UICONTROL Campaña]** | Una campaña es un conjunto de experiencias diseñadas para lograr un objetivo específico. | Al filtrar la tabla Experiencias por campaña, las métricas del resumen de todas las experiencias de la campaña pueden ser diferentes a la fila de resumen de la campaña en la vista [!UICONTROL Canales]. Esta discrepancia puede producirse si el origen del canal, como Meta y GenStudio, utiliza cálculos de resumen ligeramente diferentes. |
| **[!UICONTROL Ubicaciones]** | Un recuento de las [ubicaciones](#ad-placements) del anuncio, ubicaciones en las que apareció una experiencia en la campaña. | Las ubicaciones aumentan el alcance de la audiencia.<p>Los anuncios que no muestran ninguna ubicación ni ningún recurso pueden indicar un [tipo de anuncio no admitido](#unsupported-placements).</p> |
| **[!UICONTROL Assets]** | El número de recursos utilizados en el anuncio o la experiencia. | El recuento de la tabla Experiencias puede ser diferente al recuento de la vista Detalles de la experiencia. Esta discrepancia puede producirse si el origen del canal, como Meta y GenStudio, utiliza cálculos de resumen ligeramente diferentes. |
| **[!UICONTROL Impresiones]** | Un recuento de cada vez que la ubicación del anuncio o la experiencia se carga en el canal, independientemente de la interacción o visualización. | Un recuento alto de impresiones puede indicar una visibilidad amplia, pero para obtener una verdadera perspectiva de rendimiento, considérala en relación con otras métricas de participación. |
| **[!UICONTROL Clics]** | El número de veces que los usuarios interactúan con un elemento en el que se puede hacer clic, como un vínculo o un botón de llamada a la acción, en una ubicación de experiencia. | Un alto número de clics indica un fuerte interés y participación en el contenido, que puede ser eficaz y llegar a la audiencia adecuada. |
| **[!UICONTROL tasa de pulsaciones ]**<br>_CTR_ | Porcentaje (%) de impresiones que generaron clics en la ubicación de la experiencia dentro de una campaña.<br>**Cálculo**: `clicks` dividido por `impressions` | Una alta tasa de clics indica que el contenido es muy relevante y motivador para la audiencia en cuanto a mensajería y diseño, y que se dirige de manera efectiva a los intereses de la audiencia. |
| **[!UICONTROL CPM ]**<br>_Costo por mil_ | Coste por cada mil impresiones de publicidad para la ubicación de la experiencia.<br>**Cálculo**: importe total `spent` dividido por alcance y luego multiplicado por 1000 | Un valor bajo puede indicar una visibilidad rentable, especialmente cuando se asocia con una tasa de pulsaciones alta. |
| **[!UICONTROL CPA ]**<br>_Costo por acción_ | Coste promedio empleado para lograr una acción específica del cliente, como una compra o suscripción.<br>**Cálculo**: importe total `spent` dividido por el número de acciones del cliente completadas | Se utiliza para supervisar el gasto en experiencias que resultan en valiosas acciones del cliente. |
| **[!UICONTROL CPC ]**<br>_Costo por clic_ | Coste promedio asociado con cada clic en una ubicación de experiencia.<br>**Cálculo**: importe total `spent` dividido entre `clicks` | Unos costes medios menores pueden indicar un gasto publicitario rentable, especialmente en comparación con un aumento de las conversiones. |
| **[!UICONTROL Gasto]** | La cantidad gastada del presupuesto durante un período de tiempo determinado. | Un gasto elevado en un período corto puede indicar un uso rápido, lo que podría dar lugar a un agotamiento prematuro de los recursos. Realice un seguimiento de la cantidad gastada con métricas de rendimiento clave para ayudar a monitorizar la rentabilidad general de la inversión. |

## Rendimiento de ubicación

En la vista _Detalles de la experiencia_, las tres métricas principales reflejan el rendimiento general de la experiencia seleccionada. Sin embargo, la sección _Rendimiento por ubicación_ muestra las métricas detalladas para cada ubicación de anuncio. La siguiente tabla proporciona definiciones para métricas de rendimiento de ubicación:

| Métrica | Definición | Cálculo |
| ---------------------- | ----------------------------- | ----------- |
| **[!UICONTROL tasa de pulsaciones ]**<br>_CTR_ | Porcentaje (%) de impresiones que generaron clics en la ubicación de publicidad de la experiencia. | `clicks` dividido por `impressions` |
| **[!UICONTROL CPA ]**<br>_Costo por acción_ | Coste promedio empleado en la colocación de este anuncio para lograr una acción específica del cliente, como una compra o suscripción. | importe total `spent` dividido por el número de acciones del cliente completadas |
| **[!UICONTROL CPC ]**<br>_Costo por clic_ | Coste promedio asociado con cada clic en una ubicación de experiencia. | importe total `spent` dividido entre `clicks` |
| **[!UICONTROL Gasto]** | La cantidad gastada del presupuesto durante un período de tiempo determinado. | |
