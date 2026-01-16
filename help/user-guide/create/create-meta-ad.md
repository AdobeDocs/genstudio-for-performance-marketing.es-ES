---
title: Crear una experiencia de Meta Ad
description: Aprenda a crear experiencias de publicidad de Meta en la marca (para Facebook o Instagram) con Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 42111bbf-70cd-4fd2-a7a9-15abe072d720
source-git-commit: 168ea3d21f5771aeb05553ffe992dc9648b0e4e4
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 0%

---

# Crear una experiencia de anuncio de Meta

Este tutorial muestra cómo generar [experiencias de anuncios de Meta de marca](/help/user-guide/create/meta-experiences.md) con GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icono de pincel en el área de navegación izquierda).

Antes de empezar a generar una experiencia de anuncio de Meta, es importante [incorporar directrices](/help/user-guide/guidelines/add-guidelines.md) en GenStudio for Performance Marketing y familiarizarse con los conceptos básicos de [creación de un mensaje](/help/user-guide/effective-prompts.md).

## Elija una plantilla

Para empezar a generar una nueva experiencia publicitaria de Meta, utilice una plantilla disponible para proporcionar el marco de trabajo para el contenido. Consulte [Directrices de plantillas de anuncios de Meta](/help/user-guide/templates/meta-template.md) para obtener información sobre las proporciones de aspecto de anuncios de Meta compatibles.

Al seleccionar una plantilla, tiene la opción de utilizar una de las plantillas cargadas o una plantilla de inicio.

**Para elegir una plantilla de anuncio de Meta**:

1. En _[!DNL Create]_, haga clic en **[!UICONTROL Meta ads]**.
1. Seleccione **[!UICONTROL Plantillas personalizadas]** para examinar las plantillas cargadas o **[!UICONTROL Plantillas iniciales]** para examinar las plantillas creadas previamente.

   Si planea agregar recursos de vídeo a las variantes de Meta, debe elegir una plantilla de inicio. Están precargadas con áreas de contenido definidas por el sistema que facilitan el uso de vídeos.

1. Haga clic para seleccionar una plantilla y luego haga clic en **[!UICONTROL Usar]**.

   Esta acción abre el lienzo, que es el centro de trabajo para la creación de contenido.

## Añadir parámetros

Añadir [directrices](/help/user-guide/guidelines/overview.md) y recursos en _Parámetros_ en el cajón de solicitud mejora el proceso de generación de contenido y es un paso crucial en la preparación para generar un anuncio de Meta.

Si usa una plantilla con directrices predefinidas (como [!DNL Brands], [!DNL Personas] o [!DNL Products]), estas directrices se aplican a las variantes. Si lo desea, puede cambiarlos.

**Para agregar parámetros y recursos**:

1. Haga clic en el icono _Parameters_ para expandir el cajón de mensajes.
1. En la sección _Parameters_, seleccione las directrices—[!DNL Brands], [!DNL Personas] y [!DNL Products]—para informar sobre la creación de contenido.

   ![Elegir persona](/help/assets/persona-select-meta2.png){width="300" align="center" zoomable="yes"}

   Si no hay marcas, personalidades o productos disponibles en estos menús, [agregue directrices a su GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Agregue contenido (imágenes o vídeos) para usar en la experiencia *y* para influir en la generación de contenido:
   * Haga clic en **[!UICONTROL Seleccionar del contenido]** para seleccionar recursos del repositorio [!DNL Content], filtrar y seleccionar una o más imágenes.

     Si utiliza una plantilla que tiene una sección para vídeos, el contenido de vídeo (.mp4) se preseleccionará y filtrará por usted. Pase el ratón sobre un vídeo para ver una previsualización reproducida automáticamente.

     ![Elegir contenido visual](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

     Para usar recursos de un repositorio [!DNL AEM Assets Content Hub] conectado, elija un repositorio en el menú desplegable _Ubicación_. Filtre y seleccione una o varias imágenes.

   * O bien, arrastre y suelte imágenes en la sección **[!UICONTROL Seleccionar del contenido]** para cargar uno o más recursos nuevos.

1. Haga clic en **[!UICONTROL Usar]**.

Cuando haya terminado de agregar parámetros, puede contraer el cajón de mensajes si vuelve a hacer clic en el icono _Parámetros_.

## Introduzca una solicitud

Una vez seleccionadas las directrices, cree un mensaje con lenguaje natural para empezar a generar contenido para la nueva experiencia publicitaria de Meta. Las indicaciones detalladas generan un resultado de mayor calidad que las indicaciones vagas o ambiguas.

Consulte [Escribir mensajes efectivos](/help/user-guide/effective-prompts.md) para obtener más información sobre cómo escribir mensajes.

**Para escribir un mensaje**:

1. Escriba una solicitud en el cuadro de solicitud _&quot;Describa las experiencias que desea generar&quot;_.
1. Haga clic en **[!UICONTROL Generar]**.

   Consulte [Administrar vídeos](#manage-videos) para saber cómo se generan y cómo administrarlos.

De forma predeterminada, se generan y muestran en el lienzo cuatro variaciones (todas alimentadas por el mensaje, las directrices y el contenido añadido).

El contenido generado se carga progresivamente: a medida que se generan todas las secciones de las experiencias de Meta, estas aparecen en el lienzo. Consulte [experiencias de Meta](/help/user-guide/create/meta-experiences.md#progressive-loading) para saber cómo se cargan los cambios en el lienzo.

## Elija el canal de anuncios de Meta

Al generar un anuncio de Meta, puede elegir entre anuncios de Facebook o Instagram.

Alterne la opción de canal de anuncios de Meta (entre **Facebook** e **Instagram**) en la barra de menú derecha (iconos de Facebook e Instagram) para ver y administrar las variantes de cada canal.

Al [revisar los anuncios de Meta](#revise-generated-variants), puede cambiar la proporción de aspecto de los anuncios de Facebook e Instagram.

## Revisar variantes generadas

Antes de seleccionar qué enviar para su aprobación o publicación a [!DNL Content], puede editar los anuncios de Meta o eliminar una variante del conjunto de anuncios generados.

Para resaltar una capa individual para revisarla, haga clic en un campo o imagen editable y luego en _[!UICONTROL Ver capas]_.

**Para revisar las variantes generadas**:

* **Para [editar el nombre del borrador del anuncio de Meta](/help/user-guide/create/manage-variants.md#change-draft-name)**, haz clic en el título de _Borrador sin título_ en la parte superior del lienzo y escribe un nuevo título.
* **Para [editar manualmente un anuncio de Meta](/help/user-guide/create/manage-variants.md#manually-edit-text)**, haga clic en cualquiera de las secciones de anuncios (como la línea de asunto,
encabezado o copia de cuerpo) y edite según sea necesario.
* **Para cambiar o seleccionar call to action**, haga clic en el botón call-to-action y seleccione las opciones de texto de botón disponibles. En _Vínculo_, escriba una dirección URL para el texto de call-to-action.
* **Para [aplicar formato de texto](/help/user-guide/create/manage-variants.md#manually-edit-text)** en una variante, haz clic en el texto en la imagen o en el vínculo en línea de una variante y haz clic en **[!UICONTROL Dar formato al texto]**.
<!-- **To [change or select the Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**, click the call-to-action button and select _[!UICONTROL Rephrase]_ or _[!UICONTROL Add link]_. -->
* **Para [agregar un vínculo a una imagen en una variante](/help/user-guide/create/manage-variants.md#add-image-link)**, haga clic en un recurso de imagen (o en el área del recurso de imagen si la imagen no existe actualmente) y haga clic en el icono de vínculo.
* **Para [cambiar el tamaño y la proporción de aspecto del anuncio](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**, haga clic en el botón _[!UICONTROL Cambiar tamaño]_ (cuadro con un icono de botón en el lado izquierdo del lienzo) y seleccione un nuevo tamaño y proporción de aspecto para aplicar a todas las variantes. Las variantes se duplican y se cambia su tamaño.
* **Para [regenerar una sección de una variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, haga clic en un campo de texto editable y use las opciones _[!UICONTROL Ediciones sugeridas]_ o escriba una nueva solicitud y haga clic en **[!UICONTROL Generar]**.
* **Para [agregar o intercambiar imágenes en una variante](/help/user-guide/create/manage-variants.md#swap-image)**, haga clic en un recurso de imagen (o en el área del recurso de imagen si todavía no existe una imagen) y haga clic en el icono **[!UICONTROL Intercambiar desde contenido]**.
* **Para [recortar o cambiar la posición de las imágenes](/help/user-guide/create/manage-variants.md#crop-assets)**, haga clic en una imagen, haga clic en **[!UICONTROL Editar]** (icono de lápiz) y, a continuación, en **[!UICONTROL Recortar]**. Ajuste el tamaño y la ubicación de la imagen.
* **Para [usar Generative Expand para cambiar el tamaño y ajustar las imágenes](/help/user-guide/create/manage-variants.md#use-generative-expand) a su plantilla de trabajo**, haga clic en una imagen, haga clic en **[!UICONTROL Editar]** (icono de lápiz) y luego en **[!UICONTROL Expandir]**. Ajuste la imagen para ajustar la proporción de aspecto y la plantilla necesarias.
* **Para [agregar texto alternativo para imágenes en una variante](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**, haga clic en un recurso de imagen y use la opción _Texto alternativo_ para agregar o generar texto alternativo manualmente por imagen.
* **Para [agregar etiquetas de accesibilidad](/help/user-guide/create/manage-variants.md#add-accessibility-labels) a las variantes**, haga clic en una imagen o en un vínculo de call-to-action y, a continuación, proporcione una breve descripción que explique lo que hace el vínculo o el botón.
* **Para [eliminar un anuncio de Meta](/help/user-guide/create/manage-variants.md#delete-variant)**, haz clic en el menú de opciones de una variante y haz clic en **[!UICONTROL Eliminar variante]**.

### Administrar vídeos

Pase el ratón sobre cada uno de los vídeos para ver la reproducción automática en bucle.

Los vídeos se reenmarcan para ajustarse a la relación de aspecto seleccionada durante la generación. Para volver al vídeo original sin reenmarcar, haz clic en **[!UICONTROL Reenmarcar vídeo]** y desactívalo.

## Enviar comentarios de generación

Para [enviar comentarios](/help/user-guide/create/manage-variants.md#generation-feedback) sobre la calidad de la salida de generación, haga clic en el icono de opciones (tres puntos) y seleccione **[!UICONTROL Buena salida]** o **[!UICONTROL Mala salida]**.

## Verificar alineación de comprobación de contenido

Para optimizar las variantes generadas y garantizar el cumplimiento estricto de la identidad de marca, las directrices de plataforma y los estándares de accesibilidad, aproveche la potencia del panel [_Comprobación de contenido_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Este panel muestra detalles completos de comprobación de contenido e ilumina las áreas de mejora.

**Para realizar comprobaciones de contenido en una variante**:

1. Haga clic en el icono del panel _Comprobación de contenido_ en la barra de acciones derecha para abrir el panel [_Comprobación de contenido_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Vea un resumen de las comprobaciones de *Necesidades de revisión* y *Superado* para ver qué secciones y directrices necesitan mejorarse.

   ![_Comprobación de contenido_ panel](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [Revise manualmente las variantes](#revise-generated-variants) para asegurarse de que las variantes estén alineadas con las comprobaciones de contenido realizadas.

Consulte [Validación de marca](/help/user-guide/guidelines/brand-validation.md).

## Obtener revisiones y aprobaciones

Utilice el panel Aprobaciones, accesible como icono en la barra de acciones derecha del lienzo, para obtener críticas, realizar un seguimiento de los comentarios de revisión y obtener aprobaciones de las partes interesadas.

**Para obtener revisiones y aprobaciones**:

1. [Iniciar una solicitud de aprobación](/help/user-guide/approvals/request-review.md) para solicitar una [aprobación de las experiencias de anuncios de Meta &#x200B;](/help/user-guide/approvals/approve-content.md) redactadas.

   ![Enviar borradores para su revisión y aprobación](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. [Quitar o agregar revisores](/help/user-guide/approvals/review-and-edit.md#manage-approvals) durante el proceso de revisión.
1. [Acceda al contenido para revisarlo](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) y vea las solicitudes de revisión.
1. Edite los borradores por comentarios de revisión y [publique sus experiencias de anuncios de Meta](#publish-and-export-experience).

Consulte [Revisiones y aprobaciones](/help/user-guide/approvals/overview.md) para obtener más información.

## Publicar y exportar experiencias

Para que los anuncios de Meta generados estén disponibles para su uso actual y futuro, publíquelo en [!UICONTROL Contenido] y expórtelo para su uso en campañas de marketing.

1. **Para publicar tus nuevas experiencias publicitarias de Meta**, haz clic en **[!UICONTROL Publicar]** en la barra de herramientas superior o dentro del flujo de aprobaciones.
1. **Para exportar las nuevas experiencias de anuncios de Meta**, haga clic en **[!UICONTROL Exportar]** en la barra de herramientas superior.
   1. Seleccione el formato (HTML e imágenes o CSV e imágenes (JPG o PNG)) y haga clic en **[!UICONTROL Exportar]**.

Consulte [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) para obtener más información.

## Conectar Meta

Puede conectar GenStudio for Performance Marketing a Meta para recibir análisis avanzados y perspectivas sobre el rendimiento del contenido.

Ver [Meta ads connect](/help/user-guide/connectors/meta-ads.md).
