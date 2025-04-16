---
title: Crear una experiencia de anuncio en pantalla
description: Aprenda a crear experiencias de anuncios en pantalla en Adobe [!DNL GenStudio] for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 7d5e777b-7a30-48f4-b253-9823e38eecce
source-git-commit: a9da9ba1e93335896640e52837cc7226ec8e4bef
workflow-type: tm+mt
source-wordcount: '1024'
ht-degree: 0%

---

# Crear una experiencia de anuncio en pantalla

Este tutorial muestra cómo generar [experiencias de anuncios en pantalla](display-ad-experiences.md) de marca mediante GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icono de pincel en el área de navegación izquierda).

Para diseñar una experiencia atractiva de anuncios en pantalla, se recomienda [agregar directrices a GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) y revisar los [conceptos básicos para escribir avisos](/help/user-guide/effective-prompts.md) antes de empezar.

## Elija una plantilla

Para crear una experiencia de anuncio en pantalla, utilice una plantilla disponible para proporcionar el marco de trabajo para el contenido. Consulte [Prácticas recomendadas para plantillas](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) para obtener información acerca de las dimensiones de anuncios en pantalla admitidas.

**Para elegir una plantilla de anuncio en pantalla**:

1. En _[!DNL Create]_, haga clic en **[!UICONTROL Mostrar anuncios]**.
1. Utilice la opción de búsqueda, adyacente a _Filter_, para encontrar una plantilla de anuncio en pantalla específica.
1. En la vista _Seleccionar plantilla_, haga clic en una plantilla de anuncio en pantalla.
1. Haga clic en **[!UICONTROL Usar]**.

   Se muestra el lienzo, que sirve como centro para la creación de contenido.

## Añadir parámetros

Añadir [directrices](/help/user-guide/guidelines/overview.md) y recursos en _Parámetros_ en el cajón de solicitud sobrecarga el proceso de generación de contenido y es un paso preparatorio integral para generar una experiencia de anuncio en pantalla.

Si usa una plantilla con directrices predefinidas—[!DNL Brands], [!DNL Personas] o [!DNL Products]—estas directrices se aplican a las variantes. Si lo desea, puede cambiarlos.

**Para agregar parámetros y recursos**:

1. Haga clic en el icono _Parameters_ para expandir el cajón de mensajes.
1. En la sección _Parameters_, seleccione las directrices—[!DNL Brands], [!DNL Personas] y [!DNL Products]—para informar sobre la creación de contenido.

   Si no hay marcas, personalidades o productos disponibles en estos menús, [agregue directrices a su GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Para agregar contenido para utilizarlo en la experiencia *y* para influir en la generación de contenido:
   * Haga clic en **[!UICONTROL Seleccionar del contenido]** para seleccionar recursos (imágenes) del repositorio [!DNL Content], filtrar y seleccionar una o más imágenes.

     Para usar recursos de un repositorio [!DNL AEM Assets Content Hub] conectado, elija un repositorio en el menú desplegable _Ubicación_. Filtre y seleccione una o varias imágenes.

   * O bien, arrastre y suelte los recursos en la sección **[!UICONTROL Seleccionar del contenido]** para cargar uno o más recursos nuevos.
1. Haga clic en **[!UICONTROL Usar]**.

Cuando haya terminado de agregar parámetros, contraiga el cajón de mensajes haciendo clic de nuevo en el icono _Parameters_.

## Introduzca una solicitud

Una vez seleccionadas las directrices, cree un mensaje con lenguaje natural para empezar a generar contenido para la nueva experiencia de anuncio en pantalla. Para mejorar la calidad de las experiencias de anuncios en pantalla generadas, es crucial crear indicadores detallados y descriptivos.

![Escriba un mensaje](/help/assets/prompt-displayad.png){width="650" zoomable="yes"}

Consulte [Escribir mensajes efectivos](/help/user-guide/effective-prompts.md) para obtener más información sobre cómo escribir mensajes.

**Para escribir un mensaje**:

1. Escriba una solicitud en el cuadro de solicitud _&quot;Describa las experiencias que desea generar&quot;_.
1. Haga clic en **[!UICONTROL Generar]**.

De forma predeterminada, se generan y muestran en el lienzo cuatro variaciones (impulsadas por el mensaje, las directrices y el contenido añadido).

## Revisar variantes generadas

Antes de seleccionar qué enviar para su aprobación o publicación a [!DNL Content], puede editar las secciones de anuncios en pantalla y los campos de texto, o eliminar una variante generada.

Para resaltar una capa individual para revisarla, haga clic en un campo o imagen editable y luego en _[!UICONTROL Ver capas]_.

**Para revisar las variantes generadas**:

* **Para [editar el nombre del borrador del anuncio para mostrar](/help/user-guide/create/manage-variants.md#change-draft-name)**, haga clic en el título de _Borrador sin título_ en la parte superior del lienzo y escriba un nuevo título.
* **Para [editar manualmente un anuncio en pantalla](/help/user-guide/create/manage-variants.md#manually-edit-text)**, haga doble clic en cualquiera de las secciones o campos de anuncios en pantalla (como la línea de asunto, el encabezado o la copia de cuerpo) y edítelo según sea necesario.
* **Para [volver a generar una sección de una variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, haga clic en un campo de texto editable y use las opciones _[!UICONTROL Ediciones sugeridas]_ o escriba un nuevo mensaje en _[!UICONTROL Generar nuevo texto_ sección] y haga clic en **[!UICONTROL Generar]**.
* **Para [agregar o intercambiar imágenes en una variante](/help/user-guide/create/manage-variants.md#swap-image)**, haga clic en un recurso de imagen (o en el área del recurso de imagen si todavía no existe una imagen) y haga clic en el icono **[!UICONTROL Intercambiar desde contenido]**.
* **Para [agregar un vínculo a una imagen en una variante](/help/user-guide/create/manage-variants.md#add-image-link)**, haga clic en un recurso de imagen (o en el área del recurso de imagen si la imagen no existe actualmente) y haga clic en el icono de vínculo.
* **Para [cambiar el tamaño y la proporción de aspecto del anuncio](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**, haga clic en el botón _[!UICONTROL Cambiar tamaño]_ (cuadro con un icono de botón en el lado izquierdo del lienzo) y seleccione un nuevo tamaño y proporción de aspecto para aplicar a todas las variantes. Las variantes se duplican y se cambia su tamaño.
* **Para [recortar o cambiar la posición de las imágenes](/help/user-guide/create/manage-variants.md#crop-assets)**, pase el ratón sobre la imagen, haga clic en el icono de recorte que aparece y ajuste el tamaño y la ubicación de la imagen. Haga clic en **[!UICONTROL Aplicar]**.

<!-- # Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

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

1. [Inicie una solicitud de aprobación](/help/user-guide/approvals/request-review.md) para solicitar una [aprobación de las experiencias de anuncios en pantalla redactadas](/help/user-guide/approvals/approve-content.md).
1. [Quitar o agregar revisores](/help/user-guide/approvals/review-and-edit.md#manage-approvals) durante el proceso de revisión.
1. [Acceda al contenido para revisarlo](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) y vea las solicitudes de revisión.
1. Edite los borradores por comentarios de revisión y [publique sus experiencias de anuncios en pantalla](#publish-and-export-experience).

Ver [revisiones y aprobaciones](/help/user-guide/approvals/overview.md).

## Publicar y exportar experiencias

Para que los anuncios en pantalla generados estén disponibles para su uso actual y futuro, publíquelo en [!UICONTROL Contenido] y expórtelo para su uso en campañas de marketing.

1. **Para publicar tus nuevas experiencias con anuncios en pantalla**, haz clic en **[!UICONTROL Publicar]** en la barra de herramientas superior o dentro del flujo de aprobaciones.
   1. Seleccione _[!UICONTROL [!DNL Campaigns]]_y agregue_[!UICONTROL  más detalles ]_si lo desea.
   1. Haga clic en **[!UICONTROL Publicar]**.

      ![Publicar un anuncio para mostrar](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **Para exportar las nuevas experiencias de anuncios en pantalla**, haga clic en **[!UICONTROL Exportar]** en la barra de herramientas superior.
   1. Seleccione el formato HTML e imágenes, PNG o JPG y haga clic en **[!UICONTROL Exportar]**.

      La HTML exportada debe colocarse dentro de una propiedad web predefinida, como una plantilla o un contenedor de `div`. Sin estas cotas definidas, las imágenes pueden aparecer distorsionadas cuando se visualizan de forma independiente.

Ver [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
