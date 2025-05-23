---
title: Administración de recursos y experiencias
description: Simplifique y mejore la administración de los recursos aprobados por la marca para usarlos y reutilizarlos en su recorrido de marketing digital.
feature: Content Management, Content Attributes
exl-id: e2ce8797-6d3b-46d4-b12f-f5f80e26c669
source-git-commit: 1df977edbca284e67a5d28a6835bf5fc5608aa33
workflow-type: tm+mt
source-wordcount: '1489'
ht-degree: 1%

---

# Administración de recursos y experiencias

Adobe GenStudio for Performance Marketing [!DNL Content] simplifica y mejora la administración de los recursos aprobados por la marca para su uso y reutilización en el recorrido de marketing digital.

## [!DNL Content] galería

La galería muestra un inventario de recursos, experiencias o plantillas aprobados según la vista seleccionada. La opción de filtro (canal) situada encima de la parte izquierda de la tabla abre el menú **[!UICONTROL Filtro]**, en el que puede seleccionar entre muchas categorías para filtrar el contenido mostrado en la galería. En la vista _[!UICONTROL Assets]_, haga clic en el icono de búsqueda (lupa) para usar una palabra clave para encontrar un recurso.

A continuación se muestra una búsqueda del término `space` en la galería [!UICONTROL Assets]:

![Vista de Assets con búsqueda en el espacio](/help/assets/content-assets-filter.png "Buscando recursos con atributo de espacio")

### Buscar contenido

La interfaz de filtro y búsqueda es rápida y adaptable, y proporciona una experiencia productiva de búsqueda en primer lugar. Cada vista de [!DNL Content] proporciona opciones de filtro para restringir la búsqueda del recurso, la experiencia o la plantilla ideales. Para los recursos y las experiencias, puede seleccionar una campaña y directrices específicas, como el contenido creado para un producto específico.

Hay filtros basados en [directrices](/help/user-guide/guidelines/overview.md), [palabras clave](asset-details.md#user-defined-metadata) y [categorías de atributos](/help/user-guide/insights/attributes.md#categories) para reducir los resultados de búsqueda. Por ejemplo: es posible que desee encontrar un recurso de un tipo de archivo o tema en particular para que le ayude a crear una nueva experiencia para su campaña. O puede filtrar el contenido en función de su nombre de usuario o el nombre de un miembro del equipo:

- **[!UICONTROL Cargado por]**: limita la lista de _[!UICONTROL Assets]_ para mostrar solamente los recursos cargados por usted o por una persona específica.
- **[!UICONTROL Creado por]**: limita la lista de _[!UICONTROL Experiencias]_ para mostrar únicamente las experiencias creadas por usted o por una persona específica.
- **[!UICONTROL Plantilla]**: limita la lista _[!UICONTROL Experiencias]_ para mostrar solo las experiencias creadas con la plantilla seleccionada.

Si determinadas opciones de filtro no están visibles, indica que ninguna plantilla del repositorio coincide con los criterios de metadatos correspondientes. Asegúrese de que las plantillas estén etiquetadas correctamente con los metadatos para que se puedan detectar a través de estos filtros.

**Para buscar contenido para reutilizarlo**:

1. En _[!DNL Content]_, seleccione la sección **[!UICONTROL Assets]**.

1. Seleccione un repositorio de recursos de la lista **[!UICONTROL Ubicación]** o verifique que está viendo el repositorio de recursos correcto. `GenStudio assets` es el repositorio predeterminado.

   >[!IMPORTANT]
   >
   >La lista _Ubicación_ solo está disponible cuando [se conecta a un repositorio de AEM](connect-aem-repo.md).

1. Haga clic en **[!UICONTROL Buscar]** (lupa) para escribir una palabra clave o descripción.

1. Reduzca la búsqueda seleccionando una categoría de la lista _[!UICONTROL Filtro]_. Por ejemplo, si está buscando un archivo PNG, haga clic en **[!UICONTROL Formato de archivo]** y elija **PNG**.

   Cuanto más limitada sea la búsqueda, menos opciones de filtro estarán disponibles. Haga clic en **[!UICONTROL Borrar todo]** para eliminar todos los filtros.

1. Seleccione un recurso para obtener una vista completa y una lista de detalles.

   Haga clic en **[!UICONTROL Descargar]** (flecha abajo) para usar el recurso en la estación de trabajo local.

### Ubicación

De manera predeterminada, los recursos que agrega a [!DNL Content] a través del proceso [!DNL Create] o de la carga se almacenan en el repositorio `GenStudio assets`. El repositorio `GenStudio assets` es de lectura y escritura en GenStudio for Performance Marketing. Esto significa que puede guardar, editar y eliminar recursos en el repositorio `GenStudio assets`.

La lista **[!UICONTROL Ubicación]** sobre la galería _[!UICONTROL Assets]_ a la derecha permite seleccionar entre repositorios de Adobe Experience Manager (AEM) conectados [!DNL Assets Content Hub].

![Lista de ubicaciones de repositorios](/help/assets/content-location-selection.png "Seleccione un repositorio de contenido"){width="350"}

Al seleccionar un repositorio de AEM, la galería muestra un inventario de los recursos de ese repositorio, lo que le permite aprovechar los recursos aprobados de estos repositorios como entradas para la creación de contenido. Las opciones de filtro cambian para reflejar las categorías configuradas en [!DNL AEM Assets Content Hub].

Consulte [Conectar un repositorio de AEM](connect-aem-repo.md) para obtener instrucciones sobre cómo agregar el repositorio [!DNL AEM Assets Content Hub] a GenStudio for Performance Marketing.

El repositorio de AEM es de solo lectura, lo que significa que puede acceder al contenido, pero no puede guardar borradores, nuevos recursos ni metadatos en el repositorio de AEM. Todos los borradores y las actualizaciones finales de los recursos, las experiencias y las plantillas se guardan en el repositorio `GenStudio assets` con los nuevos [metadatos del sistema](asset-details.md#system-metadata).

{{note-aem-assets}}

Un repositorio de AEM puede aplicar ciertos requisitos de licencia, como la caducidad de los recursos. Es posible que estos recursos no estén disponibles para su uso en [!DNL Create] flujos de trabajo. Es posible que haya que renovar o reemplazar los recursos caducados para mantener la continuidad de los proyectos. Consulte a su administrador de [!DNL AEM Assets Content Hub] para obtener ayuda con estos recursos.

## Administración de Assets

En [!UICONTROL Contenido], puede almacenar, recuperar y administrar fácilmente sus recursos digitales. Al aprovechar el repositorio `GenStudio assets` y los repositorios de AEM, puede asegurarse de que los recursos estén bien organizados y sean accesibles para diversas campañas de marketing. Este enfoque de varios repositorios proporciona flexibilidad y control sobre el uso de los recursos en todos los entornos, lo que garantiza que solo se utilicen recursos aprobados y actualizados en las actividades de marketing.

En la tabla siguiente se enumeran las tareas de administración disponibles para los recursos, las experiencias y las plantillas:

| Tareas | Recursos | Experiencias | Plantillas |
| --------------------------------------------------------- | :----: | :---------: | :-------: |
| [Ver detalles](/help/user-guide/content/asset-details.md) | ✓ | ✓ | ✓ |
| [Crear experiencia](/help/user-guide/create/overview.md) |        |             | ✓ |
| [Editar en Adobe Express](#edit-in-express) | ✓ |             |           |
| [Exportar experiencias](#export-experiences) |        | ✓ |           |
| [Actualizar](/help/user-guide/content/use-templates.md#refresh-template) |   |      | ✓ |
| [Descargar](#download-assets) | ✓ |             | ✓ |
| [Eliminar](#delete-assets) | ✓ | ✓ | ✓ |

### Añadir recursos

Al agregar recursos a [!DNL Content], se almacenan de forma predeterminada en el repositorio `GenStudio assets`. El botón _[!UICONTROL Agregar recursos]_ solo está disponible cuando la _[!UICONTROL ubicación]_ es el repositorio `GenStudio assets`.

![Campo de ubicación](/help/assets/content-location.png "Campo de ubicación"){width="350"}

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

### Descarga de recursos

**Para descargar un recurso**:

1. En _[!DNL Content]_, seleccione un recurso o una plantilla. Al hacer clic en un recurso, se abre una vista enfocada del recurso.

1. En la vista de recursos, haga clic en el icono **[!UICONTROL Descargar]** (flecha hacia abajo) en la esquina superior derecha.

1. La descarga comienza a colocar una copia del recurso en la ubicación de descarga predeterminada.

### Eliminar recursos

**Para eliminar un recurso**:

1. En _[!DNL Content]_, seleccione un recurso, experiencia o plantilla. Al hacer clic en un recurso, se abre una vista enfocada del recurso.

1. En la vista de recursos, haga clic en **[!UICONTROL Eliminar]** (papelera) en la esquina superior derecha.

1. En la ventana emergente _Eliminar recurso_, verifique el recurso y haga clic en **[!UICONTROL Eliminar]**.

## Exportar experiencias

Puede seleccionar una o varias experiencias aprobadas para descargarlas en un formato compatible con el canal de destino. El nombre del archivo descargado se indica mediante la fecha de exportación: `2025-06-15-export.zip`. Al descomprimir el archivo, existe una carpeta para cada tipo de canal que incluye los recursos exportados en los formatos seleccionados. Cada recurso exportado conserva su nombre de recurso original como nombre de archivo.

**Para exportar o descargar experiencias**:

1. En _[!DNL Content]_, seleccione una o más experiencias.

   Aparece un banner con el número de experiencias seleccionadas a la izquierda y las opciones [!UICONTROL Activar], [!UICONTROL Descargar] o [!UICONTROL Eliminar] a la derecha.

1. (Opcional) Si elige activar, es posible que se le pida que seleccione una plataforma y continúe con el flujo de trabajo [!DNL Activate]. Consulte [Activar](/help/user-guide/activation/overview.md).

1. Haga clic en **[!UICONTROL Descargar]**.

1. En la ventana emergente _Descargar_, seleccione uno de los formatos disponibles.

   Si ha seleccionado varias experiencias de diferentes canales, tiene la oportunidad de seleccionar el formato para cada tipo de canal.

   - Correo electrónico, LinkedIn: `HTML`, `CSV`
   - Meta, titular y anuncio en pantalla: `HTML`, `JPEG`, `PNG`

   ![Descargar experiencias](/help/assets/content-bulk-export.png "Descargar experiencias múltiples"){width=350}

## Editar en Express

Puede editar recursos de imagen (JPG o PNG) directamente en GenStudio for Performance Marketing mediante Adobe Express. El lienzo _[!UICONTROL Powered by Adobe Express]_ proporciona funciones prácticas para mejorar tus imágenes sin salir de la aplicación GenStudio. Puede quitar fondos fácilmente, aplicar rellenos generativos, ajustar efectos y recortar imágenes.

>[!BEGINSHADEBOX]

Criterios para mejorar imágenes con la característica [!DNL Edit in Adobe Express]:

- Los tipos MIME admitidos son `image/png` y `image/jpeg`
- Las dimensiones mínimas de la imagen son de 50 x 50 píxeles
- Las dimensiones máximas de la imagen son de 8000 x 8000 píxeles
- El tamaño máximo es 40 MB (40 000 000 bytes)

>[!ENDSHADEBOX]

**Para editar un recurso con Express**:

1. En _[!DNL Content]_, seleccione un recurso de imagen. Al hacer clic en un recurso, se abre una vista enfocada del recurso.

1. En la vista de recursos, haga clic en el icono **[!UICONTROL Editar en Adobe Express]** en la esquina superior derecha.

1. En el lienzo _[!UICONTROL Powered by Adobe Express]_, usa los controles Express del panel izquierdo para mejorar tu imagen.

1. Cuando esté satisfecho con la imagen actualizada, haga clic en **[!UICONTROL Guardar una copia]** en la esquina superior derecha.

1. Seleccione el formato de archivo (JPG o PNG) y haga clic en **[!UICONTROL Guardar una copia]**.

1. En la ventana emergente _[!UICONTROL Guardar una copia del recurso]_, actualice **[!UICONTROL Nombre del recurso]**.

   - Seleccione **[!UICONTROL Mismos detalles que el recurso original]** para transferir los detalles del recurso a la nueva imagen.

   - Expanda la sección **[!UICONTROL Más detalles]** para actualizar las directrices y otros metadatos.

   >[!TIP]
   >
   >Cuantos más detalles proporcione, más experimentará las sólidas capacidades de GenStudio for Performance Marketing. Seleccione uno o más detalles de la lista o introduzca uno nuevo cuando corresponda, por ejemplo, con palabras clave. Cada detalle que agregue aparecerá debajo de la lista. Haga clic **`x`** para eliminar un detalle.

1. Haga clic en **[!UICONTROL Guardar]**.
