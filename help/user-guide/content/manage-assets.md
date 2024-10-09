---
title: Administración de recursos y experiencias
description: Simplifique y mejore la administración de los recursos aprobados por la marca para usarlos y reutilizarlos en su recorrido de marketing digital.
feature: Content, Assets, Experiences
exl-id: e2ce8797-6d3b-46d4-b12f-f5f80e26c669
source-git-commit: ce08231cb723bec3d80a732837b72a435d3b552d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Administración de recursos y experiencias

Adobe GenStudio for Performance Marketing [!DNL Content] simplifica y mejora la administración de los recursos aprobados por la marca para su uso y reutilización en el recorrido de marketing digital.

## Galería de Assets

La galería [!UICONTROL Assets] muestra un inventario de recursos aprobados. El icono de filtro (canal) situado encima de la parte izquierda de la tabla abre el menú **[!UICONTROL Filtro]**, en el que puede seleccionar entre muchas categorías para filtrar los recursos que se muestran en la galería. Haga clic en el icono de búsqueda (lupa) para utilizar una palabra clave para encontrar un recurso.

A continuación se muestra una búsqueda del término `dog` en la galería [!UICONTROL Assets]:

![Vista de Assets con búsqueda en perro](../../assets/content-assets.png)

### Ubicación de Assets

De manera predeterminada, los recursos que agrega a [!DNL Content] a través del proceso [!DNL Create] o de la carga se almacenan en el repositorio `GenStudio assets`. El repositorio `GenStudio assets` es de lectura y escritura en GenStudio for Performance Marketing. Esto significa que puede guardar, editar y eliminar recursos en el repositorio `GenStudio assets`.

La lista **[!UICONTROL Ubicación]** situada encima de la galería en el lado derecho le permite seleccionar entre repositorios de Adobe Experience Manager AEM () [!DNL Assets Content Hub] conectados. AEM Al seleccionar un repositorio de, la galería muestra un inventario de los recursos de ese repositorio, lo que le permite aprovechar los recursos aprobados de estos repositorios como entradas para la creación de contenido. Las opciones de filtro cambian para reflejar las categorías configuradas en [!DNL AEM Assets Content Hub].

AEM AEM El repositorio de datos es de solo lectura, lo que significa que no puede guardar borradores, nuevos recursos ni metadatos en el repositorio de datos de la biblioteca de datos de la biblioteca de recursos (). Todos los borradores y las actualizaciones finales de los recursos, las experiencias y las plantillas se guardan en el repositorio `GenStudio assets` con los nuevos [metadatos del sistema](asset-details.md#system-metadata).

AEM Consulte [Conectar un repositorio de](connect-aem-repo.md) para obtener instrucciones sobre cómo agregar el repositorio [!DNL AEM Assets Content Hub] a GenStudio for Performance Marketing.

## Administración de Assets

En [!UICONTROL Contenido], los especialistas en marketing de rendimiento pueden almacenar, recuperar y administrar fácilmente sus recursos digitales. AEM Al aprovechar tanto el repositorio `GenStudio assets` como los repositorios de la, los usuarios pueden asegurarse de que sus recursos estén bien organizados y sean accesibles para diversas campañas de marketing. Este enfoque de varios repositorios proporciona flexibilidad y control sobre el uso de los recursos en todos los entornos, lo que garantiza que solo se utilicen recursos aprobados y actualizados en las actividades de marketing.

### Añadir recursos

Al agregar recursos a [!DNL Content], se almacenan de forma predeterminada en el repositorio `GenStudio assets`. El botón _[!UICONTROL Agregar recursos]_ solo está disponible cuando la _[!UICONTROL ubicación]_ es el repositorio `GenStudio assets`.

![Campo de ubicación](../../assets/content-location.png){width="350" align="center"}

**Para agregar uno o más recursos**:

1. En _[!DNL Content]_, haga clic en **[!UICONTROL Agregar recursos]**.

1. En la vista _Agregar los recursos aprobados_, suelte uno o varios archivos en el espacio de colocación. Opcionalmente, puede seleccionar entre archivos locales mediante **[!UICONTROL Examinar]** o importar archivos desde Dropbox o Microsoft OneDrive.

1. En la sección _Agregar detalles_, seleccione un **[!UICONTROL nombre de campaña]** o escriba un nombre nuevo.

1. Para mejorar la capacidad de detección, agregue detalles opcionales como _Nombre de marca_, _Personas_, _Región_ y _Palabras clave_ en la sección **Más detalles**.

   Cuantos más detalles proporcione, más experimentará las sólidas capacidades de GenStudio for Performance Marketing. Seleccione uno o más detalles de la lista o introduzca uno nuevo cuando corresponda, por ejemplo, con palabras clave. Cada detalle que agregue aparecerá debajo de la lista. Haga clic **`x`** para eliminar un detalle.

   Los detalles que agregue se aplicarán a todos los recursos agregados en esta acción.

   Ver [detalles de metadatos](/help/user-guide/content/asset-details.md#system-metadata).

1. Haga clic en **[!UICONTROL Agregar recursos]**.

1. Cuando finalice la carga del recurso, haga clic en **Listo**.

1. Para ver los nuevos recursos que has cargado, haz clic en **[!UICONTROL Actualizar]** en la notificación _Nuevos recursos disponibles_ que aparece en la parte inferior del lienzo.

<!-- 
In the future, need guidance on template upload errors. For now, the UI just says error.
-->

### Buscar contenido

La interfaz de filtro y búsqueda es rápida y adaptable, y proporciona una experiencia productiva de búsqueda en primer lugar. Cada vista de [!DNL Content] proporciona opciones de filtro para restringir la búsqueda del recurso, la experiencia o la plantilla ideales. Para los recursos y las experiencias, puede seleccionar una campaña y directrices específicas, como el contenido creado para un producto específico.

Hay filtros basados en [keywords](asset-details.md#user-defined-metadata) y [atributos](/help/user-guide/insights/attributes.md) para reducir los resultados de búsqueda. Por ejemplo: es posible que desee encontrar un recurso de un tipo de archivo o tema en particular para que le ayude a crear una nueva experiencia para su campaña.

Al buscar _Experiencias_, puede usar el filtro **[!UICONTROL Creado por]** para limitar la lista y mostrar únicamente las experiencias creadas por usted o por una persona específica.

**Para buscar contenido para reutilizarlo**:

1. En _[!DNL Content]_, seleccione la sección **[!UICONTROL Assets]**.

1. Seleccione un repositorio de recursos de la lista **[!UICONTROL Ubicación]** o verifique que está viendo el repositorio de recursos correcto. `GenStudio assets` es el repositorio predeterminado.

   >[!IMPORTANT]
   >
   >AEM La lista _Ubicación_ solo está disponible cuando [te conectas a un repositorio de](connect-aem-repo.md).

1. Haga clic en **[!UICONTROL Buscar]** (lupa) para escribir una palabra clave o descripción.

1. Reduzca la búsqueda seleccionando una categoría de la lista _[!UICONTROL Filtro]_. Por ejemplo, si está buscando un archivo PNG, haga clic en **[!UICONTROL Formato de archivo]** y elija **PNG**.

   Cuanto más limitada sea la búsqueda, menos opciones de filtro estarán disponibles. Haga clic en **[!UICONTROL Borrar todo]** para eliminar todos los filtros.

1. Seleccione un recurso para obtener una vista completa y una lista de detalles.

   Haga clic en **[!UICONTROL Descargar]** (flecha abajo) para usar el recurso en la estación de trabajo local.
