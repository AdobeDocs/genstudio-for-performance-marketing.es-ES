---
title: Generar imágenes
description: Cree una imagen, que coincida con el estilo de una imagen de referencia, en Adobe [!DNL GenStudio] for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="Esta función se encuentra actualmente en Beta, por lo que algunas funciones pueden estar limitadas o sujetas a cambios."
role: User
level: Beginner
recommendations: noDisplay
exl-id: c1118ada-7fee-43cd-aff4-eab69539afb4
source-git-commit: 47195c08f500e50a01db127c6badc461c10afaf9
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 0%

---

# Generar imágenes

Con el uso de GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icono de pincel), puede generar recursos generados por _[!DNL On-brand images]_&#x200B;que se inspiren en una imagen elegida, capturando su impacto visual y su estética general.<!-- [two types of images](#image-types) using GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (paintbrush icon)—_[!DNL On-brand images]_ and _[!DNL Similar images]_. -->

Para diseñar una imagen llamativa y efectiva, se recomienda [agregar directrices a GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) y revisar los [conceptos básicos para escribir avisos](/help/user-guide/effective-prompts.md).

## Tipos de imagen

_[!DNL On-brand images]_&#x200B;son recursos generados que se inspiran en una imagen elegida y capturan su impacto visual y su estética general. Estas imágenes se crean utilizando imágenes que ya están disponibles en [!DNL Content] y un mensaje cuidadosamente diseñado que guía el diseño. Siguen estrictamente tanto las directrices de marca como los parámetros elegidos durante el proceso de generación.

_[!DNL On-brand images]_<!-- and _[!DNL Similar images]_ --> incorpora directrices establecidas, parámetros y un [mensaje cuidadosamente diseñado](/help/user-guide/effective-prompts.md) para que entregue recursos de imagen llamativos.

<!-- * _[!DNL Similar images]_—Image assets created with strong similarity to an existing selected image available in [!DNL Content]. When generating similar images, GenStudio for Performance Marketing redesigns the selected image, giving slight variations on the content to provide variety and nuance. -->

## Generar imágenes en la marca

Puede generar [!DNL On-brand images] utilizando las directrices definidas, los parámetros y una imagen de referencia seleccionada. Estos elementos, junto con el mensaje, guían la generación de variaciones [!DNL On-brand image] coherentes.

### Elija una imagen de referencia

Para crear un _[!DNL On-brand images]_, seleccione una imagen existente guardada en [!DNL Content]. Consulte [Prácticas recomendadas para plantillas](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) para obtener información sobre las dimensiones [!DNL on-brand image] admitidas.

**Para elegir una imagen de referencia**:

1. En _[!DNL Create]_, haga clic en **[!UICONTROL Imagen de marca]**.
1. Utilice la opción de búsqueda, adyacente a _Filter_, para encontrar una imagen específica.

   ![Seleccionar imagen de referencia](/help/assets/select-img.png){width="400" zoomable="yes"}

   Para usar recursos de un repositorio [!DNL AEM Assets Content Hub] conectado, elija un repositorio en el menú desplegable _Ubicación_. Filtre y seleccione una imagen.

1. En la vista _Seleccionar imagen_, haga clic en una imagen.

   La imagen seleccionada puede tener un tamaño de hasta 10 mb.

1. Haga clic en **[!UICONTROL Usar]**.

   Se muestra el lienzo, que sirve como centro para la creación de contenido.

### Añadir parámetros

La incorporación de [directrices](/help/user-guide/guidelines/overview.md) y parámetros mejora el proceso de generación de contenido y es un paso preparatorio crucial para producir un [!DNL on-brand image].

**Para agregar directrices y parámetros**:

1. En la ficha _Básico_, seleccione un(a) [!DNL Brand] para informar sobre la creación de contenido.

   Si no hay marcas disponibles en este menú, [agregue directrices a su GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Seleccione la categoría de imagen que mejor se ajuste al resultado deseado en _[!UICONTROL Categoría de imagen]_.

   Las categorías de imágenes están disponibles si se seleccionó un(a) [!DNL Brand]. Las opciones están determinadas por el elemento [!DNL Brand] seleccionado.

<!-- 1. _(Optional)_ Select a custom model from _[!UICONTROL Model]_.

   Models are available if you access to [custom models in Firefly](https://adobedx.slack.com/archives/CMF1JGMLY/p1743534402774569). The _Models_ list will be blank if you do not have access. -->

1. Seleccione la proporción de aspecto que desee en _[!UICONTROL Proporción de aspecto]_.
1. Haga clic en **[!UICONTROL Seleccionar del contenido]** en _[!UICONTROL Referencia de estilo]_ para agregar una imagen de referencia. La imagen que seleccione influirá en la estética visual y en la profundidad de las imágenes que genere.

   Para usar recursos de un repositorio [!DNL AEM Assets Content Hub] conectado, elija un repositorio en el menú desplegable _Ubicación_. Filtre y seleccione una imagen.

1. En la ficha _Avanzado_, seleccione _Tipo de contenido_.

   Se preseleccionó en función de la categoría de imagen presente para el(la) [!DNL Brand]&#x200B;(el) _Arte_ o _Foto_(la) seleccionado(s)) y no se puede editar.

1. Ajuste la intensidad general de las características visuales existentes de la imagen en _[!UICONTROL Intensidad visual]_.

### Introduzca una solicitud

Después de seleccionar los parámetros, cree un mensaje utilizando un lenguaje natural para empezar a generar imágenes de marca.

Consulte [Escribir mensajes efectivos](/help/user-guide/effective-prompts.md).

**Para escribir un mensaje**:

1. Introduzca una solicitud en el cuadro de solicitud.
1. Haga clic en **[!UICONTROL Generar]**.

De forma predeterminada, se generan y muestran en el lienzo cuatro variaciones (impulsadas por el mensaje, los parámetros y el contenido añadido).

### Editar en Adobe Express

Después de generar variantes de imagen, puede editarlas directamente en Adobe GenStudio for Performance Marketing mediante Adobe Express.

**Para editar una imagen individual mediante Adobe Express**:

1. Pase el ratón sobre una variante de imagen generada y haga clic en _[!UICONTROL Editar en Adobe Express]_.

   Aparece una ventana _Con tecnología Adobe Express_.

1. Realice la edición de imágenes, como [recortar una imagen](https://helpx.adobe.com/es/express/create-and-edit-images/edit-images/crop-images.html), [quitar un objeto](https://helpx.adobe.com/es/express/create-and-edit-images/create-and-modify-with-generative-ai/remove-objects-generative-fill.html) y aplicar efectos.

   Consulte [Documentación de Adobe Express](https://helpx.adobe.com/es/express/user-guide.html) para obtener información sobre cómo revisar imágenes en GenStudio for Performance Marketing con Adobe Express.

1. Haga clic en _[!UICONTROL Aplicar cambios]_ para guardar las ediciones.
1. Siga editando las variantes de imagen individuales que desee y aplicando cambios para guardar el progreso.

### Verificar alineación de comprobación de contenido

Para optimizar las variantes generadas y garantizar el cumplimiento estricto de la identidad de marca, las directrices de plataforma y los estándares de accesibilidad, aproveche la potencia del panel [_Comprobación de contenido_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Este panel muestra detalles completos de comprobación de contenido e ilumina las áreas de mejora.

**Para realizar comprobaciones de contenido**:

1. Haga clic en el icono del panel _Comprobación de contenido_ en la barra de acciones derecha para abrir el panel [_Comprobación de contenido_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Vea un resumen de las comprobaciones de *Necesidades de revisión* y *Superado* para ver qué secciones y directrices necesitan mejorarse.

   ![_Comprobación de contenido_ panel](/help/assets/content-check-img.png){width="500" zoomable="yes"}

1. Revise las variantes de la imagen para asegurarse de que están estrechamente alineadas con las comprobaciones de contenido realizadas.

Consulte [Validación de marca](/help/user-guide/guidelines/brand-validation.md).

<!-- ## Generate Similar images

You can quickly generate images similar to a selected image within [!DNL Content] from the [!DNL Create] home.

**To create _[!DNL Similar images]_**:

1. In _[!DNL Create]_, click **[!UICONTROL Similar images]**.
1. Use the search option, adjacent to _Filter_, to find a specific image.

   To use assets from a connected [!DNL AEM Assets Content Hub] repository, choose a repository from the _Location_ drop-down menu. Filter and select one image.

1. In the _Select image_ view, click on an image.
1. Click **[!UICONTROL Use]**.

   The Canvas, which serves as the central hub for content creation, is displayed. Four image variations similar to the original selected image appear.

   ![Generate similar images](/help/assets/generate-similar.png){width="400" zoomable="yes"} -->

## Publicación y exportación de imágenes

Los borradores de imágenes generados se muestran en la sección _Recientes_ de la página de inicio [!DNL Create].

Para que las imágenes generadas estén disponibles para su uso actual y futuro, publíquelas en [!UICONTROL Contenido] y expórtelas para su uso en campañas de marketing.

1. **Para publicar tus nuevas imágenes**, haz clic en **[!UICONTROL Publicar]** en la barra de herramientas superior.
   1. _[!UICONTROL Agregar detalles]_, como _[!UICONTROL Campañas]_ o _[!UICONTROL Canales]_, si lo desea.
   1. Haga clic en **[!UICONTROL Publicar]**.

1. **Para exportar tus nuevas imágenes**, haz clic en **[!UICONTROL Exportar]** en la barra de herramientas superior.
   1. Seleccione el formato (JPG o PNG) y haga clic en **[!UICONTROL Exportar]**.

Ver [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
