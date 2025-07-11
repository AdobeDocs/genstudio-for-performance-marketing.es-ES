---
title: Crear una experiencia de LinkedIn
description: Aprenda a crear experiencias de LinkedIn compatibles con la marca con Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
badgeBeta: label="Beta" tooltip="Esta función se encuentra actualmente en Beta, por lo que algunas funciones pueden estar limitadas o sujetas a cambios."
recommendations: noDisplay
exl-id: abe10fc8-d6d5-4cad-9273-400b622f22b7
source-git-commit: d82891b2347c6b97bf8f6eef9cffe363ea341725
workflow-type: tm+mt
source-wordcount: '1224'
ht-degree: 0%

---

# Crear una experiencia de LinkedIn

Este tutorial muestra cómo generar [experiencias LinkedIn](/help/user-guide/create/meta-experiences.md) que se ajusten a las directrices de marca mediante GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icono de pincel en el área de navegación izquierda).

Antes de empezar a generar un anuncio de LinkedIn, es importante [agregar directrices](/help/user-guide/guidelines/add-guidelines.md) en GenStudio for Performance Marketing y conocer los conceptos básicos de [creación de un mensaje](/help/user-guide/effective-prompts.md).

## Elija una plantilla

Para generar una nueva experiencia de LinkedIn, necesita una plantilla para proporcionar el marco de trabajo para el contenido. Consulte [Directrices de la plantilla LinkedIn](/help/user-guide/templates/linkedin-template.md) para obtener información sobre las proporciones de aspecto de LinkedIn admitidas.

Puede seleccionar de la lista de plantillas personalizadas o elegir una plantilla de inicio.

**Para elegir una plantilla de LinkedIn**:

1. En _[!DNL Create]_, haga clic en **[!UICONTROL LinkedIn]**.
1. Seleccione **[!UICONTROL Plantillas personalizadas]** para examinar las plantillas cargadas o **[!UICONTROL Plantillas iniciales]** para examinar las plantillas creadas previamente.

   Si planea agregar recursos de vídeo a las variantes Meta, debe elegir una plantilla de inicio. Están precargadas con áreas de contenido definidas por el sistema que facilitan el uso de vídeos.

1. Haga clic para seleccionar una plantilla y luego haga clic en **[!UICONTROL Usar]**.

   Esta acción abre el lienzo, que es el centro de trabajo para la creación de contenido.

## Añadir parámetros

Añadir [directrices](/help/user-guide/guidelines/overview.md) y recursos en _Parámetros_ en el cajón de solicitud mejora el proceso de generación de contenido y es un paso crucial en la preparación para generar una experiencia de LinkedIn.

**Para agregar parámetros y recursos**:

1. Haga clic en el icono _Parameters_ para expandir el cajón de mensajes.
1. En la sección _Parameters_, seleccione las directrices—[!DNL Brands], [!DNL Personas] y [!DNL Products]—para informar sobre la creación de contenido.

   ![Elegir persona](/help/assets/persona-select.png){width="600" zoomable="yes"}

   Si no hay marcas, personalidades o productos disponibles en estos menús, [agregue directrices a su GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Agregue contenido (imágenes o vídeos) para usar en la experiencia *y* para influir en la generación de contenido haciendo clic en **[!UICONTROL Seleccionar entre los contenidos]**. O bien, arrastre y suelte imágenes en la sección **[!UICONTROL Seleccionar del contenido]** para cargar uno o más recursos nuevos.

   Utilice el filtro para buscar contenido y seleccionar una o más imágenes.

   Si utiliza una plantilla que tiene una sección para vídeos, el contenido de vídeo (.mp4) se preseleccionará y filtrará por usted. Pase el ratón sobre un vídeo para ver una previsualización reproducida automáticamente.

   ![Elegir contenido visual](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

   Para usar recursos de un repositorio [!DNL AEM Assets Content Hub] conectado, elija un repositorio en el menú desplegable _Ubicación_. Filtre y seleccione una o varias imágenes.

1. Haga clic en **[!UICONTROL Usar]**.

Cuando haya terminado de agregar parámetros, puede contraer el cajón de mensajes si vuelve a hacer clic en el icono _Parámetros_.

## Introduzca una solicitud

Después de seleccionar las directrices, cree un mensaje con lenguaje natural para empezar a generar contenido para la nueva experiencia de LinkedIn. Las instrucciones detalladas garantizan la buena calidad y la utilidad de la salida.

Consulte [Escribir mensajes efectivos](/help/user-guide/effective-prompts.md) para obtener más información sobre cómo escribir mensajes.

**Para escribir un mensaje**:

1. Escriba una solicitud en el cuadro de solicitud _&quot;Describa las experiencias que desea generar&quot;_.
1. Haga clic en **[!UICONTROL Generar]**.

   Consulte [Administrar vídeos](#manage-videos) para saber cómo se generan y cómo administrarlos.

De forma predeterminada, se generan y muestran en el lienzo cuatro variaciones (todas alimentadas por el mensaje, las directrices y el contenido añadido).

El contenido generado se carga progresivamente: a medida que se generan todas las secciones de las experiencias de LinkedIn, estas aparecen en el lienzo. Vea [experiencias de LinkedIn](/help/user-guide/create/linkedin-experiences.md#progressive-loading) para saber cómo se cargan esos cambios en el lienzo.

## Revisión de anuncios de LinkedIn generados

Antes de enviar variantes para su aprobación o publicación en [!DNL Content], puede editar los anuncios de LinkedIn o eliminar una variante del conjunto de anuncios generados.

**Para revisar las variantes generadas**:

* **Para [editar el nombre del borrador del anuncio de LinkedIn](/help/user-guide/create/manage-variants.md#change-draft-name)**, haga clic en el título de _Borrador sin título_ en la parte superior del lienzo e introduzca un nuevo título.
* **Para [editar manualmente un anuncio de LinkedIn](/help/user-guide/create/manage-variants.md#manually-edit-text)**, haga clic en cualquiera de las secciones de anuncios (como la línea de asunto, el encabezado o la copia del cuerpo) y edítela según sea necesario.
* **Para cambiar o seleccionar call to action**, haga clic en el botón call-to-action y seleccione las opciones de texto de botón disponibles. En _Vínculo_, escriba una dirección URL para el texto de call-to-action.
* **Para [aplicar formato de texto](/help/user-guide/create/manage-variants.md#manually-edit-text)** en una variante, haga clic en el texto en la imagen de una variante y haga clic en **[!UICONTROL Dar formato al texto]**.
* **Para [volver a generar una sección de una variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, haga clic en un campo de texto editable y use las opciones _[!UICONTROL Ediciones sugeridas]_ o escriba un nuevo mensaje en _[!UICONTROL Generar nuevo texto_ sección] y haga clic en **[!UICONTROL Generar]**.
* **Para [usar Generative Expand para cambiar el tamaño y ajustar las imágenes](/help/user-guide/create/manage-variants.md#use-generative-expand) a su plantilla de trabajo**, haga clic en una imagen, haga clic en **[!UICONTROL Editar]** (icono de lápiz) y luego en **[!UICONTROL Expandir]**. Ajuste la imagen para ajustar la proporción de aspecto y la plantilla necesarias.
* **Para [recortar o cambiar la posición de las imágenes](/help/user-guide/create/manage-variants.md#crop-assets)**, pase el ratón sobre una imagen, haga clic en el icono de recorte que aparece y ajuste el tamaño y la ubicación de la imagen.
* **Para [cambiar el tamaño y la proporción de aspecto del anuncio](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**, haga clic en el botón _[!UICONTROL Cambiar tamaño]_ (cuadro con un icono de botón en el lado izquierdo del lienzo) y seleccione un nuevo tamaño y proporción de aspecto para aplicar a todas las variantes. Las variantes se duplican y se cambia su tamaño.
* **Para [agregar o intercambiar recursos (imagen o vídeo) en una variante](/help/user-guide/create/manage-variants.md#swap-image)**, haga clic en un recurso (o en el área de recursos) y haga clic en el icono **[!UICONTROL Intercambiar del contenido]**.
* **Para [agregar texto alternativo para imágenes en una variante](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**, haga clic en un recurso de imagen y use la opción _Texto alternativo_ para agregar o generar texto alternativo manualmente por imagen.
* **Para [agregar etiquetas de accesibilidad](/help/user-guide/create/manage-variants.md#add-accessibility-labels) a las variantes**, haga clic en una imagen o en un vínculo de call-to-action y, a continuación, proporcione una breve descripción que explique lo que hace el vínculo o el botón.
* **Para [eliminar un anuncio de LinkedIn](/help/user-guide/create/manage-variants.md#delete-variant)**, haz clic en el menú de opciones de una variante y haz clic en **[!UICONTROL Eliminar variante]**.

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

1. [Revise manualmente las variantes](#revise-generated-linkedin-ads) para asegurarse de que sus variantes estén alineadas con las comprobaciones de contenido completadas.

Consulte [Validación de marca](/help/user-guide/guidelines/brand-validation.md).

## Obtener revisiones y aprobaciones

Utilice el panel Aprobaciones, al que se puede acceder desde la barra de menú superior del lienzo, para obtener críticas, realizar un seguimiento de los comentarios de las revisiones y obtener las aprobaciones de las partes interesadas.

**Para obtener revisiones y aprobaciones**:

1. [Inicie una solicitud de aprobación](/help/user-guide/approvals/request-review.md) para solicitar una [aprobación de las experiencias de anuncio Meta ](/help/user-guide/approvals/approve-content.md).

   ![Enviar borradores para su revisión y aprobación](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. [Quitar o agregar revisores](/help/user-guide/approvals/review-and-edit.md#manage-approvals) durante el proceso de revisión.
1. [Acceda al contenido para revisarlo](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) y vea las solicitudes de revisión.
1. Edite los borradores por comentarios de revisión y [publique sus experiencias de anuncio Meta](#publish-and-export-experience).

Consulte [Revisiones y aprobaciones](/help/user-guide/approvals/overview.md) para obtener más información.

## Publicar y exportar experiencias

Para que los anuncios de LinkedIn generados estén disponibles para su uso actual y futuro, publíquelo en [!UICONTROL Contenido] y expórtelo para su uso en campañas de marketing.

1. **Para publicar sus nuevas experiencias**, haga clic en **[!UICONTROL Publicar]** en la barra de herramientas superior o dentro del flujo de aprobaciones.
1. **Para exportar tus nuevas experiencias**, haz clic en **[!UICONTROL Exportar]** en la barra de herramientas superior.
   1. Seleccione el formato JPG, PNG o GIF y haga clic en **[!UICONTROL Exportar]**.

Consulte [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) para obtener más información.
