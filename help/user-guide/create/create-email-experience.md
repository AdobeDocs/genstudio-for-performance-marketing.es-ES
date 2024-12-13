---
title: Crear una experiencia de correo electrónico
description: Aprenda a crear experiencias de correo electrónico en Adobe GenStudio for Performance Marketing.
feature: Content, Brands Service, Guidelines, Content Generation, Create, Experiences, Variant Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 34446202-da98-45ff-869a-b43496a477f8
source-git-commit: 763c907598d92779483938295a99d640ee3f4d20
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 0%

---

# Crear una experiencia de correo electrónico

Este tutorial muestra cómo generar [experiencias de correo electrónico](/help/user-guide/create/email-experiences.md) de marca mediante GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icono de pincel en el área de navegación izquierda).

Para crear una experiencia de correo electrónico efectiva, se recomienda [agregar directrices a GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) y profundizar en los [conceptos básicos para escribir un mensaje](/help/user-guide/effective-prompts.md) antes de comenzar.

## Elija una plantilla

Para crear una nueva experiencia de correo electrónico, utilice una plantilla disponible para proporcionar el marco de trabajo para el contenido.

**Para elegir una plantilla de correo electrónico**:

1. En _[!DNL Create]_, haga clic en **[!UICONTROL Correo electrónico]**en_&quot;¿Qué desea crear hoy?&quot;_sección.
1. Utilice la opción de búsqueda, adyacente a _Filter_, para encontrar una plantilla de correo electrónico específica.
1. Haga clic para seleccionar una plantilla de correo electrónico y haga clic en **[!UICONTROL Usar]**.

   Aparece Canvas, el epicentro de la creación de contenido.

## Añadir parámetros

Añadir [directrices](/help/user-guide/guidelines/overview.md) y recursos en _Parámetros_ en el cajón de solicitud sobrecarga el proceso de generación de contenido y es un paso preparatorio integral para generar una experiencia de correo electrónico.

**Para agregar parámetros y recursos**:

1. Haga clic en el icono _Parameters_ para expandir el cajón de mensajes.
1. En la sección _Parameters_, seleccione las directrices—[!DNL Brands], [!DNL Personas] y [!DNL Products]—para informar sobre la creación de contenido.

   ![Elegir persona](/help/assets/persona-select.png){width="600" zoomable="yes"}

   Si no hay marcas, personalidades o productos disponibles en estos menús, [agregue directrices a su GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Agregue contenido para utilizarlo en la experiencia *y* para influir en la generación de contenido:
   * Haga clic en **[!UICONTROL Seleccionar del contenido]** para seleccionar recursos (imágenes) del repositorio [!DNL Content], filtrar y seleccionar una o más imágenes.

     ![Elegir contenido visual](/help/assets/content-select-email.png){width="500" zoomable="yes"}

     Para usar recursos de un repositorio [!DNL AEM Assets Content Hub] conectado, elija un repositorio en el menú desplegable _Ubicación_. Filtre y seleccione una o varias imágenes.

   * O bien, arrastre y suelte los recursos en la sección **[!UICONTROL Seleccionar del contenido]** para cargar uno o más recursos nuevos.
1. Haga clic en **[!UICONTROL Usar]**.

>[!NOTE]
>Si la plantilla de correo electrónico tiene varias secciones, seleccione [!DNL Products] y el contenido (recursos visuales) de cada sección de correo electrónico en _Correos electrónicos de varias secciones_. Los correos electrónicos de varias secciones admiten un recurso visual por sección. Solo puede agregar recursos visuales a correos electrónicos de varias secciones desde [!DNL Content]; no puede arrastrar y soltar ni cargar recursos desde su origen local.
>![Agregar contenido y parámetros para cada sección de correo electrónico ](/help/assets/parameters-multisection-email.png){width="450" zoomable="yes"}

Cuando haya terminado de agregar parámetros, puede contraer el cajón de mensajes si vuelve a hacer clic en el icono _Parámetros_.

## Introduzca una solicitud

Una vez seleccionadas las directrices, cree un mensaje con lenguaje natural para empezar a generar contenido para la nueva experiencia de correo electrónico. Las indicaciones detalladas generan un resultado de mayor calidad que las indicaciones vagas o indescriptivas.

Consulte [Escribir mensajes efectivos](/help/user-guide/effective-prompts.md) para obtener más información sobre cómo escribir mensajes.

**Para escribir un mensaje**:

1. Escriba una solicitud en el cuadro de solicitud _&quot;Describa las experiencias que desea generar&quot;_.
1. Haga clic en **[!UICONTROL Generar]**.

De forma predeterminada, se generan y muestran en el lienzo cuatro variaciones (todas alimentadas por el mensaje, las directrices y el contenido añadido).

El contenido generado se carga progresivamente: a medida que se generan todas las secciones de las experiencias de correo electrónico, estas aparecen en el lienzo. Consulte [Experiencias de correo electrónico](/help/user-guide/create/meta-experiences.md#progressive-loading) para saber cómo se cargan los cambios en el lienzo.

## Revisar correos electrónicos generados

Antes de seleccionar lo que se enviará para su aprobación o publicación en [!DNL Content], puede editar las secciones de correo electrónico o eliminar una variante del conjunto de correos electrónicos generados.

**Para revisar las variantes generadas**:

* **Para [editar el nombre del borrador del correo electrónico](/help/user-guide/create/manage-variants.md#change-draft-name)**, haga clic en el título de _Borrador sin título_ en la parte superior del lienzo y escriba un nuevo título.
* **Para [editar manualmente un correo electrónico](/help/user-guide/create/manage-variants.md#manually-edit-text)**, haga clic en cualquiera de los campos de texto editables (como la línea de asunto, el encabezado o la copia de cuerpo) y edítelo según sea necesario
* **Para [regenerar una sección de una variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, haga clic en un campo de texto editable y use las opciones _[!UICONTROL Ediciones sugeridas]_ o escriba una nueva solicitud y haga clic en **[!UICONTROL Generar]**.
* **Para [agregar o intercambiar imágenes en una variante](/help/user-guide/create/manage-variants.md#swap-image)**, haga clic en un recurso de imagen (o en el área del recurso de imagen si todavía no existe una imagen) y haga clic en **[!UICONTROL Seleccionar o intercambiar a partir del contenido]** o **[!UICONTROL Cargar nueva imagen]** para agregar o intercambiar una imagen en una variante individual.
* **Para [eliminar un correo electrónico](/help/user-guide/create/manage-variants.md#delete-variant)**, haga clic para seleccionar el título del correo electrónico (por ejemplo, &quot;Correo electrónico 1/4&quot;) y haga clic en **[!UICONTROL Eliminar variante]**.

## Enviar comentarios de generación

Para [enviar comentarios](/help/user-guide/create/manage-variants.md#generation-feedback) sobre la calidad de la salida de generación, haga clic en el icono de opciones (tres puntos) y seleccione **[!UICONTROL Buena salida]** o **[!UICONTROL Mala salida]**.

## Vista previa del dispositivo

Al revisar y preparar experiencias por correo electrónico, puede [alternar entre vistas previas para escritorio y vistas móviles](/help/user-guide/create/manage-variants.md#preview-for-device) para garantizar la coherencia y el atractivo visual de las variantes de borrador.

## Verificar alineación de marca

Para optimizar los mensajes de correo electrónico generados y garantizar el cumplimiento estricto de la identidad de marca, aproveche la potencia de la [_comprobación de las directrices de marca_](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) (que proporciona un resumen de la alineación de marca para una variante) y del panel [_Validación de marca_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) (que muestra detalles completos de validación de marca y áreas de mejora ilustrativas).

**Para comprobar la alineación de marca**:

1. Haga clic en el icono [**[!UICONTROL [!DNL Brand] directrices para buscar una variante ]**](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) y vea un resumen del rendimiento de esa variante cuando se compara con su marca.

   ![Comprobación de las directrices de marca](/help/assets/brand-guidelines-check.png){width="350" zoomable="yes"}

1. Para obtener los detalles de las secciones y directrices que deben mejorarse, haga clic en **[!UICONTROL Revisar]** _o_ haga clic en el icono Validación de marca en la barra de menú superior para abrir el [_Panel de validación de marca_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel).

1. Desplácese por cada correo electrónico para ver cómo puede mejorar el contenido generado y alinearlo mejor con la marca.

   ![Panel de validación de marca](/help/assets/brand-validation-panel.png){width="600" zoomable="yes"}

1. [Revisa manualmente los correos electrónicos](#revise-generated-emails) para asegurarte de que estén alineados con tu marca.

Consulte [Validación de marca](/help/user-guide/guidelines/brand-validation.md).

## Obtener revisiones y aprobaciones

Utilice el panel Aprobaciones, al que se puede acceder desde la barra de menú superior del lienzo, para obtener críticas, realizar un seguimiento de los comentarios de las revisiones y obtener las aprobaciones de las partes interesadas.

**Para obtener revisiones y aprobaciones**:

1. [Iniciar una solicitud de aprobación](/help/user-guide/approvals/request-review.md) para solicitar una [aprobación de las experiencias de correo electrónico con borrador](/help/user-guide/approvals/approve-content.md).
1. [Quitar o agregar revisores](/help/user-guide/approvals/review-and-edit.md#manage-approvals) durante el proceso de revisión.
1. [Acceda al contenido para revisarlo](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) y vea las solicitudes de revisión.
1. Edite los borradores por comentarios de revisión y [publique sus experiencias de correo electrónico](#publish-and-export-experience).

Consulte [Revisiones y aprobaciones](/help/user-guide/approvals/overview.md) para obtener más información.

## Publish y experiencia de exportación

Para que los mensajes de correo electrónico generados estén disponibles para su uso actual y futuro, publíquelos en [!UICONTROL Contenido] y expórtelos para su uso en campañas de marketing.

1. **Para publicar tus nuevas experiencias de correo electrónico**, haz clic en **[!UICONTROL Publish]** en la barra de herramientas superior o dentro del flujo de aprobaciones.
1. **Para exportar las nuevas experiencias de correo electrónico**, haga clic en **[!UICONTROL Exportar]** en la barra de herramientas superior.
   1. Seleccione el formato (solo CSV e imágenes o HTML) y haga clic en **[!UICONTROL Exportar]**.

Consulte [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) para obtener más información.
