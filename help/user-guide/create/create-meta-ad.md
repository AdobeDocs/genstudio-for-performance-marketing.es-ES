---
title: Crear una experiencia de Meta ad
description: Aprenda a crear experiencias de publicidad Meta en la marca (para Facebook o Instagram) con Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 42111bbf-70cd-4fd2-a7a9-15abe072d720
source-git-commit: f49a2bd241f98dda23f6612f8c699ec49d222a12
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---

# Crear una experiencia de Meta ad

Este tutorial muestra cómo generar [experiencias de anuncios Meta](/help/user-guide/create/meta-experiences.md) de marca mediante GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icono de pincel en el área de navegación izquierda).

Antes de empezar a generar una experiencia de anuncio Meta, es importante [incorporar directrices](/help/user-guide/guidelines/add-guidelines.md) en GenStudio for Performance Marketing y familiarizarse con los conceptos básicos de [creación de un mensaje](/help/user-guide/effective-prompts.md).

## Elija una plantilla

Para empezar a generar una nueva experiencia de publicidad de metadatos, utilice una plantilla disponible para proporcionar el marco de trabajo para el contenido. Consulte [Prácticas recomendadas para plantillas](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) para obtener información sobre las proporciones de aspecto de metadatos y publicidad admitidas.

**Para elegir una plantilla Meta ad**:

1. En _[!DNL Create]_, haga clic en **[!UICONTROL Meta ads]**.
1. Utilice la opción de búsqueda, adyacente a _Filter_, para encontrar una plantilla de anuncio Meta específica.
1. Haga clic para seleccionar una plantilla y luego haga clic en **[!UICONTROL Usar]**.

   Esta acción abre el lienzo, que es el centro de trabajo para la creación de contenido.

## Añadir parámetros

Añadir [directrices](/help/user-guide/guidelines/overview.md) y recursos en _Parámetros_ en el cajón de solicitud mejora el proceso de generación de contenido y es un paso crucial en la preparación para generar un anuncio Meta.

Si usa una plantilla con directrices predefinidas—[!DNL Brands], [!DNL Personas] o [!DNL Products]—estas directrices se aplican a las variantes. Si lo desea, puede cambiarlos.

**Para agregar parámetros y recursos**:

1. Haga clic en el icono _Parameters_ para expandir el cajón de mensajes.
1. En la sección _Parameters_, seleccione las directrices—[!DNL Brands], [!DNL Personas] y [!DNL Products]—para informar sobre la creación de contenido.

   ![Elegir persona](/help/assets/persona-select.png){width="600" zoomable="yes"}

   Si no hay marcas, personalidades o productos disponibles en estos menús, [agregue directrices a su GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Agregue contenido para utilizarlo en la experiencia *y* para influir en la generación de contenido:
   * Haga clic en **[!UICONTROL Seleccionar del contenido]** para seleccionar recursos (imágenes) del repositorio [!DNL Content], filtrar y seleccionar una o más imágenes.

     ![Elegir contenido visual](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

     Para usar recursos de un repositorio [!DNL AEM Assets Content Hub] conectado, elija un repositorio en el menú desplegable _Ubicación_. Filtre y seleccione una o varias imágenes.

   * O bien, arrastre y suelte los recursos en la sección **[!UICONTROL Seleccionar del contenido]** para cargar uno o más recursos nuevos.
1. Haga clic en **[!UICONTROL Usar]**.

Cuando haya terminado de agregar parámetros, puede contraer el cajón de mensajes si vuelve a hacer clic en el icono _Parámetros_.

## Introduzca una solicitud

Una vez seleccionadas las directrices, cree un mensaje con lenguaje natural para empezar a generar contenido para la nueva experiencia de publicidad de Meta. Las indicaciones detalladas generan un resultado de mayor calidad que las indicaciones vagas o ambiguas.

Consulte [Escribir mensajes efectivos](/help/user-guide/effective-prompts.md) para obtener más información sobre cómo escribir mensajes.

**Para escribir un mensaje**:

1. Escriba una solicitud en el cuadro de solicitud _&quot;Describa las experiencias que desea generar&quot;_.
1. Haga clic en **[!UICONTROL Generar]**.

De forma predeterminada, se generan y muestran en el lienzo cuatro variaciones (todas alimentadas por el mensaje, las directrices y el contenido añadido).

El contenido generado se carga progresivamente: a medida que se generan cada sección de las metaexperiencias, estas aparecen en el lienzo. Vea [metaexperiencias](/help/user-guide/create/meta-experiences.md#progressive-loading) para conocer cómo se cargan esos cambios en el lienzo.

## Elija el canal Meta ads

Al generar un anuncio Meta, puede elegir entre anuncios de Facebook o Instagram.

Cambie la opción de canal Meta ads (entre **Facebook** e **Instagram**) en la barra de menú derecha (iconos de Facebook e Instagram) para ver y administrar variantes de cada canal.

Al [revisar los anuncios Meta](#revise-generated-variants), puede cambiar la proporción de aspecto de los anuncios de Facebook e Instagram.

## Revisar variantes generadas

Antes de seleccionar qué enviar para su aprobación o publicación a [!DNL Content], puede editar los anuncios Meta o eliminar una variante del conjunto de anuncios generados.

Para resaltar una capa individual para revisarla, haga clic en un campo o imagen editable y luego en _[!UICONTROL Ver capas]_.

**Para revisar las variantes generadas**:

* **Para [editar el nombre del borrador del anuncio Meta](/help/user-guide/create/manage-variants.md#change-draft-name)**, haga clic en el título de _Borrador sin título_ en la parte superior del lienzo y escriba un nuevo título.
* **Para [editar manualmente un Meta ad](/help/user-guide/create/manage-variants.md#manually-edit-text)**, haga clic en cualquiera de las secciones de anuncios (como la línea de asunto,
encabezado o copia de cuerpo) y edite según sea necesario.
* **Para cambiar o seleccionar call to action**, haga clic en el botón call-to-action y seleccione las opciones de texto de botón disponibles. En _Vínculo_, escriba una dirección URL para el texto de call-to-action.
<!-- **To [change or select the Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**, click the call-to-action button and select _[!UICONTROL Rephrase]_ or _[!UICONTROL Add link]_. -->
* **Para [agregar un vínculo a una imagen en una variante](/help/user-guide/create/manage-variants.md#add-image-link)**, haga clic en un recurso de imagen (o en el área del recurso de imagen si la imagen no existe actualmente) y haga clic en el icono de vínculo.
* **Para [regenerar una sección de una variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, haga clic en un campo de texto editable y use las opciones _[!UICONTROL Ediciones sugeridas]_ o escriba una nueva solicitud y haga clic en **[!UICONTROL Generar]**.
* **Para [agregar o intercambiar imágenes en una variante](/help/user-guide/create/manage-variants.md#swap-image)**, haga clic en un recurso de imagen (o en el área del recurso de imagen si todavía no existe una imagen) y haga clic en el icono **[!UICONTROL Intercambiar desde contenido]**.
* **Para [recortar o cambiar la posición de las imágenes](/help/user-guide/create/manage-variants.md#crop-assets)**, pase el ratón sobre una imagen, haga clic en el icono de recorte que aparece y ajuste el tamaño y la ubicación de la imagen.
* **Para [agregar texto alternativo para imágenes en una variante](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**, haga clic en un recurso de imagen y use la opción _Texto alternativo_ para agregar o generar texto alternativo manualmente por imagen.
* **Para [eliminar un Meta ad](/help/user-guide/create/manage-variants.md#delete-variant)**, haga clic en el menú de opciones de una variante y haga clic en **[!UICONTROL Eliminar variante]**.

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

1. [Inicie una solicitud de aprobación](/help/user-guide/approvals/request-review.md) para solicitar una [aprobación de las experiencias de anuncio Meta ](/help/user-guide/approvals/approve-content.md).

   ![Enviar borradores para su revisión y aprobación](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. [Quitar o agregar revisores](/help/user-guide/approvals/review-and-edit.md#manage-approvals) durante el proceso de revisión.
1. [Acceda al contenido para revisarlo](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) y vea las solicitudes de revisión.
1. Edite los borradores por comentarios de revisión y [publique sus experiencias de anuncio Meta](#publish-and-export-experience).

Consulte [Revisiones y aprobaciones](/help/user-guide/approvals/overview.md) para obtener más información.

## Publicar y exportar experiencias

Para que los anuncios Meta generados estén disponibles para su uso actual y futuro, publíquelos en [!UICONTROL Contenido] y exporte el contenido para su uso en campañas de marketing.

1. **Para publicar tus nuevas experiencias con Meta Ad**, haz clic en **[!UICONTROL Publicar]** en la barra de herramientas superior o dentro del flujo de aprobaciones.
1. **Para exportar tus nuevas experiencias con Meta Ad**, haz clic en **[!UICONTROL Exportar]** en la barra de herramientas superior.
   1. Seleccione el formato (HTML e imágenes o CSV e imágenes (JPG o PNG)) y haga clic en **[!UICONTROL Exportar]**.

Consulte [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) para obtener más información.

## Conectar Meta

Puede conectar GenStudio for Performance Marketing a Meta para recibir análisis avanzados y perspectivas sobre el rendimiento del contenido.

Ver [Meta ads connect](/help/user-guide/connectors/meta-ads.md).
