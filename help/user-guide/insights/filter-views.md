---
title: Filtrar vistas de perspectivas
description: Aprenda a utilizar las funcionalidades de filtro mejoradas con Insights.
level: Intermediate
feature: Reporting and Insights
exl-id: fbc53c2a-388c-4b51-94e2-626cd1e18e63
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '868'
ht-degree: 0%

---

# Filtro para vistas de perspectivas

El tablero [!DNL Insights] proporciona un conjunto completo de filtros para una experiencia de exploración de datos eficiente. Al analizar canales, anuncios, medios o atributos específicos, las opciones de filtrado le permiten personalizar la vista y optimizar el flujo de trabajo. Utilice filtros de palabra clave para un objetivo preciso o explore listas predefinidas para restringir la búsqueda y centrarse en los datos más importantes.

## Conceptos básicos del filtro

Cada vista de [!DNL Insights] ofrece una lista de opciones de filtro. La opción de filtro (funnel) de la izquierda abre el menú **[!UICONTROL Filtro]**. Tanto si está viendo la tabla como la galería, los filtros aplicados aparecerán en la lista **[!UICONTROL Filtrar por]** sobre la tabla o galería. De forma predeterminada, se seleccionan un canal y una cuenta.

![Filtrar por](/help/assets/insights-filter-by.png "Filtrar por"){width=600 zoomable="yes"}

Los filtros aplicados persisten en todas las vistas. Seleccione **[!UICONTROL Borrar todo]** sobre la tabla o galería para eliminar todos los filtros seleccionados.

### Campo de búsqueda

Haga clic en el icono de búsqueda (lupa) para escribir un término de búsqueda y localizar elementos específicos en la tabla o galería. Por ejemplo, al escribir el término `Gear` en la tabla [!UICONTROL Ads], se filtran los resultados para mostrar únicamente los anuncios que utilizan el término `Gear` en el nombre.

![Ejemplo de campo de búsqueda](/help/assets/insights-search.png "Buscar anuncios con engranaje en el nombre"){width=600 zoomable="yes"}

### Intervalo de fechas

El selector de intervalo de fechas es una potente herramienta para alinear los datos mostrados con los objetivos del análisis. Utilice el selector de intervalo de fechas para ajustar el lapso de tiempo de los datos mostrados en la tabla o en la vista de galería. De forma predeterminada, el intervalo de fecha se establece en los últimos 30 días. Para incluir más datos o centrarse en un periodo específico, expanda el intervalo de fechas.

![Selector de intervalo de fecha](/help/assets/insights-date-range.png "Seleccione un intervalo de fecha"){width=400}

Si no aparece ningún elemento en la tabla o en la vista de galería, puede deberse a que el intervalo de fechas seleccionado excluye los datos relevantes. En estos casos, aumente el intervalo de fechas para asegurarse de que se incluyen los datos deseados.

### Páginas

Algunas tablas pueden abarcar varias páginas, como se indica debajo de la tabla a la derecha. Utilice las versátiles opciones de búsqueda y filtrado para restringir los resultados. Para desplazarse entre páginas, utilice los controles de paginación derecha (hacia delante) e izquierda (hacia atrás). Asegúrese de aplicar los filtros correctamente para incluir todos los datos relevantes en todas las páginas.

### Control de deslizamiento

Algunas opciones de filtro incluyen un control de diapositiva, que permite seleccionar un valor dentro de un intervalo definido. Por ejemplo, en _[!UICONTROL Atributos]_, el control deslizante **[!UICONTROL Recuento de medios]** le permite filtrar atributos en función del número de imágenes o vídeos asociados. Arrastre el control deslizante para especificar un intervalo, desde un mínimo de 0 hasta un máximo que pueda superar los 100.

## Filtrado avanzado

Con los filtros _[!UICONTROL Campañas]_ y _[!UICONTROL Anuncios]_, puede aprovechar palabras clave precisas para restringir la lista. Los filtros de palabras clave son especialmente útiles para filtrar campañas o anuncios que utilizan una convención de nombres compleja con varios identificadores únicos. Por ejemplo, un nombre de campaña puede incluir lo siguiente:

- Código o nombre de región específico: `NA`, `EMEA`
- Acrónimos de tipo de contenido: `EB`, `CHT` o `DSP`
- Códigos de ofertas o siglas: `OFFER2023`, `PROMO`

Con el tiempo, su lista de campañas y anuncios puede crecer exponencialmente. Considere el siguiente escenario para usar el filtro _[!UICONTROL Campaigns]_ para restringir la tabla [!UICONTROL Ads].

**Para restringir la tabla Anuncios usando el filtro Campañas**:

1. En _[!DNL Insights]_, seleccione la vista **[!UICONTROL Anuncios]**.

   ![Filtro de anuncios y tabla](/help/assets/insights-ads-filter.png "Vista de anuncios con menú de filtro"){zoomable="yes"}

1. Haga clic en la opción de filtro (funnel) situada encima de la parte izquierda de la tabla para abrir el menú **[!UICONTROL Filtro]**.

1. Compruebe que el canal `Filter by` y la cuenta estén seleccionados correctamente.

1. Expanda el filtro **[!UICONTROL Campaigns]** y haga clic en **[!UICONTROL Select]**.

   ![Filtrar campañas](/help/assets/insights-filter-campaigns-expand.png "Expandir campañas filtrar"){width=200}

1. En el campo de búsqueda _[!UICONTROL Seleccionar campañas]_, escriba palabras clave separadas por comas.

   Utilice palabras clave para restringir la búsqueda con un filtrado lógico y preciso.

   - Para buscar nombres de campaña que contengan `adventure` **Y** `ready`, escriba ambas palabras clave separadas por una coma:

     ![Buscar todas las palabras clave](/help/assets/insights-select-campaigns-and.png "Buscar nombres de campaña que contengan ambas palabras clave"){width=500}

   - Para buscar nombres de campañas que contengan `adventure` **O** `ready`, escriba cada palabra clave por separado:

     ![Busque palabras clave](/help/assets/insights-select-campaigns-or.png "Busque nombres de campaña que contengan al menos una palabra clave"){width=500}

   - Para realizar búsquedas avanzadas, combine varios conjuntos de palabras clave. Por ejemplo, busque nombres de campañas con `adventure` y `apparel` **OR** `sun` y `gear`:

     ![Buscar con varios conjuntos de palabras clave](/help/assets/insights-advanced-or.png "Buscar nombres de campaña usando varios conjuntos de palabras clave"){width=500}

1. Seleccione una o más campañas de la búsqueda resultante y haga clic en **[!UICONTROL Aplicar]**.

   ![Lista de campañas](/help/assets/insights-select-campaigns-list.png "Seleccione campañas para incluir")

Las campañas seleccionadas aparecerán ahora en la lista _[!UICONTROL Filtrar por]_ situada encima de la tabla o galería de anuncios. Puede centrarse exclusivamente en los anuncios vinculados a las campañas seleccionadas. En este ejemplo, los resultados filtrados incluyen 6 anuncios, lo que proporciona una vista más dirigida para el análisis.

![Tabla filtrada por campañas](/help/assets/insights-filter-by-campaigns.png "Tabla con campañas filtradas"){zoomable="yes"}

Puede filtrar aún más la tabla [!UICONTROL Media] de manera similar para los nombres de anuncios. Expanda el filtro **[!UICONTROL Ads]**, haga clic en **[!UICONTROL Seleccionar]** y podrá realizar un filtro de palabras clave similar para restringir la tabla multimedia o la vista de la galería.

## Descargar resultados de tabla

Puede descargar los resultados filtrados de la vista de tabla para un análisis o uso compartido más profundos. Haga clic en el icono de descarga (flecha hacia abajo) situado sobre la parte derecha de la tabla para descargar un archivo CSV basado en la tabla visible. La descarga comienza automáticamente y coloca el archivo CSV en la ubicación de descarga predeterminada.

Algunas tablas pueden tener varias páginas, que se pueden ver debajo del lado derecho de la tabla. El archivo CSV incluye datos de _todas_ las páginas de la tabla.
