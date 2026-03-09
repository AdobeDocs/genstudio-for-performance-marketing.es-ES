---
title: Información general sobre Insights
description: Aprenda a optimizar los anuncios en función de las métricas de rendimiento de contenido en tiempo real.
level: Intermediate
feature: Reporting and Insights
exl-id: 26402a06-f776-42be-9d8d-fc498c0f75a8
TQID: https://experienceleague.adobe.com/7ERGkM2wuM8JHYf-bi-SAVMSblhwpkt7NNuUNgCCcfc
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
  - id: b03d2162-d906-40a0-9cbd-001391e22d4a
  - id: bb0d2eba-617d-4fdd-b920-2f535b5c031c
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
source-wordcount: 675
ht-degree: 0%

---

# Adobe GenStudio for Performance Marketing Insights

Adobe GenStudio for Performance Marketing [!DNL Insights] proporciona análisis avanzados y perspectivas sobre el rendimiento del contenido que pueden ayudarle a tomar decisiones basadas en datos.

En el panel [!DNL Insights], puede:

- **Identifique el contenido más efectivo**: Indique qué contenido ofrece el mejor rendimiento para diferentes audiencias y adapte el contenido o las campañas futuras para las preferencias de tendencias.
- **Optimizar contenido de bajo rendimiento**: encuentre contenido que no funcione bien y use la IA generativa integrada para crear variaciones inmediatamente, lo que podría mejorar su eficacia sin comenzar desde cero.
- **Revitalizar contenido de alto rendimiento**: tome contenido exitoso y ajústelo para actualizar el anuncio para la audiencia o adapte el contenido a pantalla completa para usarlo en nuevas campañas, lo que podría extender su ciclo de vida y rendimiento.

## Conectores de datos

La primera vez que abra [!DNL Insights], verá un banner que le guiará para conectar Adobe GenStudio for Performance Marketing con una cuenta de canal.

Esta conexión permite que GenStudio for Performance Marketing reciba datos estadísticos de sus campañas de marketing, medios y anuncios activos. Inicialmente, GenStudio for Performance Marketing ingiere los últimos 6 meses de datos para que tenga las herramientas necesarias para analizar los datos más recientes y actuar en consecuencia.

{{connect-insights}}

## Canales admitidos

Los canales admitidos en Insights son Meta, LinkedIn, TikTok, DV360 e Innovid.

Meta, LinkedIn y TikTok proporcionan una visibilidad completa de las campañas, los anuncios, los medios y los atributos. DV360 e Innovid ofrecen actualmente una cobertura de datos más limitada.

En este momento, los datos de medios no están disponibles para DV360 e Innovid, lo que significa que la pestaña Atributos tampoco se muestra para estos canales. La pestaña Atributos depende de los datos de nivel de medios para que aparezcan las características extraídas de las experiencias.

Esta limitación se debe a restricciones en las propias plataformas de medios de pago y no a un problema con GenStudio for Performance Marketing.

## Panel de control

El panel [!DNL Insights] tiene una tabla configurable para cada tipo de contenido: [!UICONTROL Canales], [!UICONTROL Anuncios], [!UICONTROL Medios] y [!UICONTROL Atributos].

![[!DNL Insights] panel](/help/assets/insights-dashboard.png)

Cada vista muestra una tabla correspondiente, en la que puede buscar por palabra clave, filtrado e intervalo de fechas. Puede hacer clic en el icono de configuración (cog) situado encima de la parte derecha de la tabla para alternar los tipos de columnas visibles. La fila _[!UICONTROL Resumen]_ puede mostrar totales o promedios de una columna.

[!UICONTROL Anuncios], [!UICONTROL Medios] y [!UICONTROL Atributos] incluyen una vista de galería que permite analizar y ordenar recursos con tarjetas con una miniatura de imagen o vídeo. Hay una opción para mostrar una de las tres métricas clave en cada tarjeta: `Click-through rate`, `Cost per click` y `Spend`.

### Campañas

La vista [[!DNL Insights] _[!UICONTROL Campañas &#x200B;]_](campaigns.md) es la vista predeterminada y muestra una lista de detalles de campañas activas, como objetivos, presupuesto, fecha de inicio y actividad. Asegúrese de [conectar una cuenta de canal](/help/user-guide/connectors/connect-channel.md) para que GenStudio for Performance Marketing empiece a recibir los datos estadísticos.

### Anuncios

La vista [[!DNL Insights] _[!UICONTROL Anuncios &#x200B;]_](ads.md) se centra en evaluar la efectividad de un anuncio. La vista [!UICONTROL Anuncios] le permite analizar las métricas de un anuncio en función de su ubicación dentro de un intervalo de fechas especificado. Al hacer clic en un&#x200B;_[!UICONTROL &#x200B; nombre del anuncio &#x200B;]_, puedes ver las métricas de rendimiento del anuncio, el rendimiento por ubicación de anuncio y los atributos.

### Medios

La vista [[!DNL Insights] _[!UICONTROL Media &#x200B;]_](media.md) está diseñada para ayudarle a analizar el rendimiento del contenido creativo. Puede identificar atributos de medios que contribuyan a mejorar una métrica seleccionada, como clics o impresiones.

Al hacer clic en el contenido multimedia, se proporciona más contexto sobre su rendimiento en diferentes anuncios y ubicaciones de anuncios:

![Detalles multimedia](/help/assets/insights-media-details.png){width="600" zoomable="yes"}

En la vista de detalles de medios, la parte izquierda muestra una miniatura del recurso y una lista de atributos. Hay tres métricas resaltadas: `Click-through rate`, `Cost per click` y `Spend`. Los aspectos destacados del rendimiento muestran cómo se comparan los valores reales (línea continua) con el valor promedio (línea de puntos) durante el período de tiempo seleccionado (el valor predeterminado es `Last 30 days`).

### Atributos

Los _atributos_ del contenido ayudan a identificar el contenido creativo mediante detalles inherentes, como el color, el tono, la composición (como el asunto, las fuentes, los elementos visuales) y otros componentes clave. Los atributos suelen ser el conjunto de información de contenido menos medido y analizado.

La vista [[!DNL Insights] _[!UICONTROL Atributos &#x200B;]_](attributes.md) puede ayudarle a investigar e identificar qué atributos funcionan mejor con determinadas audiencias, canales y regiones, así como a resaltar las tendencias estacionales. Con estas perspectivas, puede utilizar atributos de rendimiento para crear variantes, dirigirse a una audiencia específica o experimentar con diferentes estrategias de campaña.
