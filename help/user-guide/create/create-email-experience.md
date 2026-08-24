---
title: Crear una experiencia de correo electrónico
description: Aprenda a crear experiencias de correo electrónico en Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 34446202-da98-45ff-869a-b43496a477f8
TQID: https://experienceleague.adobe.com/RPeJQ02q9HXBSpn-uFqjzLCYbbzv5eNnFBXkFn9j5JI
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2: id: a8b28c00-da6e-4d27-8667-80f790ad8972id: be495d08-ecd1-455f-951e-c22de504e667id: de1f9646-abd3-4e21-9de2-df62ce55c8dcid: dee4e9a9-78d1-4953-8179-f8da6117027did: e3878dde-4b87-4290-9e81-ed7ee6eb83feid: f54ee13b-9545-4d68-9842-a12026e60aaf
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
source-git-commit: e47c6644de51ead57f1c2e780aa287eb1de7ac87
workflow-type: tm+mt
source-wordcount: 1547
ht-degree: 0%

---

# Crear una experiencia de correo electrónico

Este tutorial muestra cómo generar [experiencias de correo electrónico](/help/user-guide/create/email-experiences.md) de marca mediante GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icono de pincel en el área de navegación izquierda).

Para crear una experiencia de correo electrónico efectiva, se recomienda [agregar directrices a GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) y profundizar en los [conceptos básicos para escribir un mensaje](/help/user-guide/effective-prompts.md) antes de comenzar.

## Elija una plantilla

Para crear una nueva experiencia de correo electrónico, utilice una plantilla disponible para proporcionar el marco de trabajo para el contenido.

**Para elegir una plantilla de correo electrónico**:

1. En _[!DNL Create]_, haga clic en **[!UICONTROL Correo electrónico]**.
1. Utilice la opción de búsqueda, adyacente a _Filter_, para encontrar una plantilla de correo electrónico específica.
1. Haga clic para seleccionar una plantilla de correo electrónico y haga clic en **[!UICONTROL Usar]**.

   Aparece Canvas, el epicentro de la creación de contenido.

## Añadir parámetros

Añadir [directrices](/help/user-guide/guidelines/overview.md) y recursos en _Parámetros_ en el cajón de solicitud sobrecarga el proceso de generación de contenido y es un paso preparatorio integral para generar una experiencia de correo electrónico.

Si usa una plantilla con directrices predefinidas (como [!DNL Brands], [!DNL Personas] o [!DNL Products]), estas directrices se aplican a las variantes. Si lo desea, puede cambiarlos.

**Para agregar parámetros y recursos**:

1. Haga clic en el icono _Parameters_ para expandir el cajón de mensajes.
1. En la sección _Parameters_, seleccione las directrices—[!DNL Brands], [!DNL Personas] y [!DNL Products]—para informar sobre la creación de contenido.

   ![Elegir persona](/help/assets/persona-select-email2.png){width="50%" align="center"}

   Si no hay marcas, personalidades o productos disponibles en estos menús, [agregue directrices a su GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Agregue contenido para utilizarlo en la experiencia *y* para influir en la generación de contenido:
   * Haga clic en **[!UICONTROL Seleccionar del contenido]** para seleccionar recursos (imágenes) del repositorio [!DNL Content], filtrar y seleccionar una o más imágenes.

     ![Elegir contenido visual](/help/assets/content-select-email.png){width="500" zoomable="yes"}

     Para usar recursos de un repositorio [!DNL AEM Assets Content Hub] conectado, elija un repositorio en el menú desplegable _Ubicación_. Filtre y seleccione una o varias imágenes.

   * O bien, arrastre y suelte los recursos en la sección **[!UICONTROL Seleccionar del contenido]** para cargar uno o más recursos nuevos.
1. Haga clic en **[!UICONTROL Usar]**.

   >[!NOTE]
   >Si la plantilla de correo electrónico tiene varias secciones, seleccione [!DNL Products] y el contenido (recursos visuales) de cada sección de correo electrónico en _Correos electrónicos de varias secciones_. Los correos electrónicos de varias secciones admiten un recurso visual por sección. Solo puede agregar recursos visuales a correos electrónicos de varias secciones desde [!DNL Content]; no puede arrastrar y soltar ni cargar recursos desde su origen local.
   >![Agregar contenido y parámetros a cada sección de correo electrónico](/help/assets/parameters-multisection-email.png){width="450" zoomable="yes"}

Cuando haya terminado de agregar parámetros, puede contraer el cajón de mensajes si vuelve a hacer clic en el icono _Parámetros_.

## Introduzca una solicitud

Una vez seleccionadas las directrices, cree un mensaje con lenguaje natural para empezar a generar contenido para la nueva experiencia de correo electrónico. Las indicaciones detalladas generan un resultado de mayor calidad que las indicaciones vagas o ambiguas.

Consulte [Escribir mensajes efectivos](/help/user-guide/effective-prompts.md) para obtener más información sobre cómo escribir mensajes.

**Para escribir un mensaje**:

1. Escriba una solicitud en el cuadro de solicitud _&quot;Describa las experiencias que desea generar&quot;_.
1. Haga clic en **[!UICONTROL Generar]**.

De forma predeterminada, se generan y muestran en el lienzo cuatro variaciones (todas alimentadas por el mensaje, las directrices y el contenido añadido).

El contenido generado se carga progresivamente: a medida que se generan todas las secciones de las experiencias de correo electrónico, estas aparecen en el lienzo. Consulte [Experiencias de correo electrónico](/help/user-guide/create/meta-experiences.md#progressive-loading) para saber cómo se cargan los cambios en el lienzo.

## Revisar variantes generadas

Antes de seleccionar lo que se enviará para su aprobación o publicación en [!DNL Content], puede editar las secciones de correo electrónico o eliminar una variante del conjunto de correos electrónicos generados.

**Para revisar las variantes generadas**:

* **Para [editar el nombre del borrador del correo electrónico](/help/user-guide/create/manage-variants.md#change-draft-name)**, haga clic en el título de _Borrador sin título_ en la parte superior del lienzo y escriba un nuevo título.
* **Para [editar manualmente un correo electrónico](/help/user-guide/create/manage-variants.md#manually-edit-text)**, haga clic en cualquiera de los campos de texto editables (como la línea de asunto, el encabezado o la copia de cuerpo) y edítelo según sea necesario
* **Para usar [fragmentos de contenido aprobados en variantes de correo electrónico](/help/user-guide/create/email-experiences.md#content-fragment-swap)**, descubra cómo [!DNL GenStudio for Performance Marketing] combina campos generativos, campos de fragmentos de contenido inyectables y campos bloqueados en un lienzo. Los administradores configuran los orígenes de fragmento tal como se describe en [Buscar extensión de fragmento de contenido](/help/extensibility/deploy-app.md#find-content-fragment-extension).
* **Para [cambiar o seleccionar Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**, haga clic en el botón call-to-action y seleccione _[!UICONTROL Reformular]_ o _[!UICONTROL Agregar vínculo]_.
* **Para [aplicar formato de texto](/help/user-guide/create/manage-variants.md#manually-edit-text)** en una variante, haga clic en el texto en la imagen de una variante y haga clic en **[!UICONTROL Dar formato al texto]**.
* **Para [regenerar una sección de una variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, haga clic en un campo de texto editable y use las opciones _[!UICONTROL Ediciones sugeridas]_ o escriba una nueva solicitud y haga clic en **[!UICONTROL Generar]**.
* **Para [agregar o intercambiar imágenes en una variante](/help/user-guide/create/manage-variants.md#swap-image)**, haga clic en un recurso de imagen (o en el área del recurso de imagen si todavía no existe una imagen) y haga clic en el icono **[!UICONTROL Intercambiar desde contenido]**.
* **Para [editar una imagen en una variante](#edit-images-in-the-canvas)**, haga clic en un campo de imagen y haga clic en **[!UICONTROL Editar]** (icono de lápiz) para recortar, cambiar la posición o expandir la imagen directamente en el lienzo.
* **Para [agregar un vínculo a una imagen en una variante](/help/user-guide/create/manage-variants.md#add-image-link)**, haga clic en un recurso de imagen (o en el área del recurso de imagen si la imagen no existe actualmente) y haga clic en el icono de vínculo.
* **Para [agregar texto alternativo para imágenes en una variante](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**, haga clic en un recurso de imagen y use la opción _Texto alternativo_ para agregar o generar texto alternativo manualmente por imagen.
* **Para [agregar etiquetas de accesibilidad](/help/user-guide/create/manage-variants.md#add-accessibility-labels) a las variantes**, haga clic en una imagen o en un vínculo de call-to-action y, a continuación, proporcione una breve descripción que explique lo que hace el vínculo o el botón.
* **Para [eliminar un correo electrónico](/help/user-guide/create/manage-variants.md#delete-variant)**, haga clic para seleccionar el título del correo electrónico (por ejemplo, &quot;Correo electrónico 1/4&quot;) y haga clic en **[!UICONTROL Eliminar variante]**.

## Editar imágenes en el lienzo

Ajuste de imágenes sin salir del lienzo ni depender de herramientas de diseño externas. Puede recortar y cambiar la posición de una imagen para centrarse en un asunto o utilizar Expansión generativa para extender una imagen más allá de sus límites originales. Las ediciones solo se aplican al borrador del correo electrónico. Los recursos de Source de [!DNL Content] y los repositorios de recursos conectados nunca se modifican.

Acceda a la edición de imágenes desde cualquier campo de imagen del lienzo de correo electrónico. Las imágenes editadas se indican visualmente para que pueda rastrear qué imágenes ha cambiado del recurso original.

### Recortar y cambiar la posición de una imagen

Recorte una imagen para utilizar únicamente la región que desee. El recorte en correos electrónicos es de forma libre, sin restricciones de proporción de aspecto, por lo que tiene control total sobre qué parte de la imagen aparece y en qué proporción.

**Para recortar y cambiar la posición de una imagen**:

1. En un borrador de correo electrónico, pase el ratón sobre y haga clic en un campo de imagen.
1. Haga clic en **[!UICONTROL Editar]** (icono de lápiz).
1. Haga clic en **[!UICONTROL Recortar]**.
1. Ajuste la región de recorte y arrastre la imagen a la posición deseada.
1. Haga clic en **[!UICONTROL Aplicar]** para recortar la imagen seleccionada o en **[!UICONTROL Aplicar a todas las imágenes]** para aplicar el recorte en todos los campos de imagen del borrador.

Para salir sin guardar los cambios, haga clic en **[!UICONTROL Cancelar]**.

![La vista Editar imagen con la herramienta Recortar activa en una imagen del lienzo del correo electrónico](/help/assets/edit-image-crop-email.png){width="650" zoomable="yes"}

### Expandir una imagen con Expansión generativa

Utilice Expansión generativa para extender una imagen más allá de sus límites originales con IA generativa. La expansión del correo electrónico no se limita a un tamaño o proporción fijos, por lo que puede ajustar una imagen al espacio que necesite.

**Para expandir una imagen**:

1. En un borrador de correo electrónico, pase el ratón sobre y haga clic en un campo de imagen.
1. Haga clic en **[!UICONTROL Editar]** (icono de lápiz).
1. Haga clic en **[!UICONTROL Expandir]**.

   La imagen se abrirá en la vista _[!UICONTROL Editar imagen]_ en un lienzo expandido y [!DNL GenStudio for Performance Marketing] generará opciones de expansión.

1. Mueva la imagen para colocarla dentro del área expandida.
1. Seleccione una opción generada o haga clic en **[!UICONTROL Más]** (icono de signo más) para ver más opciones.
1. Haga clic en **[!UICONTROL Aplicar]** para aplicar el resultado a la imagen seleccionada o en **[!UICONTROL Aplicar a todas las imágenes]** para aplicarlo a todos los campos de imagen del borrador.

Para salir sin guardar los cambios, haga clic en **[!UICONTROL Cancelar]**.

>[!NOTE]
>
>El tamaño de salida de la expansión generativa no está restringido, por lo que la calidad puede variar en expansiones muy grandes. Haga clic en **[!UICONTROL Más]** para generar opciones adicionales si el resultado no satisface sus necesidades.

![Un resultado de expansión generativa seleccionado y listo para aplicarse en la vista Editar imagen](/help/assets/generative-expand-email.png){width="650" zoomable="yes"}

## Enviar comentarios de generación

Para [enviar comentarios](/help/user-guide/create/manage-variants.md#generation-feedback) sobre la calidad de la salida de generación, haga clic en el icono de opciones (tres puntos) y seleccione **[!UICONTROL Buena salida]** o **[!UICONTROL Mala salida]**.

## Vista previa del dispositivo

Al revisar y preparar experiencias por correo electrónico, puede [alternar entre vistas previas para escritorio y vistas móviles](/help/user-guide/create/manage-variants.md#preview-for-device) para garantizar la coherencia y el atractivo visual de las variantes de borrador.

## Verificar alineación de comprobación de contenido

Para optimizar las variantes generadas y garantizar el cumplimiento estricto de la identidad de marca, las directrices de plataforma y los estándares de accesibilidad, aproveche la potencia del panel [_Comprobación de contenido_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Este panel muestra detalles completos de comprobación de contenido e ilumina las áreas de mejora.

**Para realizar comprobaciones de contenido en una variante**:

1. Haga clic en el icono del panel _Comprobación de contenido_ en la barra de acciones derecha para abrir el panel [_Comprobación de contenido_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Vea un resumen de las comprobaciones de *Necesidades de revisión* y *Superado* para ver qué secciones y directrices necesitan mejorarse.

   ![_Comprobación de contenido_ panel](/help/assets/content-check-panel.png){width="300"}

2. [Revise manualmente las variantes](#revise-generated-variants) para asegurarse de que las variantes estén alineadas con las comprobaciones de contenido realizadas.

Consulte [Validación de marca](/help/user-guide/guidelines/brand-validation.md).

## Obtener revisiones y aprobaciones

Utilice el panel Aprobaciones, accesible como icono en la barra de acciones derecha del lienzo, para obtener críticas, realizar un seguimiento de los comentarios de revisión y obtener aprobaciones de las partes interesadas.

**Para obtener revisiones y aprobaciones**:

1. [Iniciar una solicitud de aprobación](/help/user-guide/approvals/request-review.md) para solicitar una [aprobación de las experiencias de correo electrónico con borrador](/help/user-guide/approvals/approve-content.md).
1. [Quitar o agregar revisores](/help/user-guide/approvals/review-and-edit.md#manage-approvals) durante el proceso de revisión.
1. [Acceda al contenido para revisarlo](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) y vea las solicitudes de revisión.
1. Edite los borradores por comentarios de revisión y [publique sus experiencias de correo electrónico](#publish-and-export-experience).

Consulte [Revisiones y aprobaciones](/help/user-guide/approvals/overview.md) para obtener más información.

## Publicar y exportar experiencias

Para que los mensajes de correo electrónico generados estén disponibles para su uso actual y futuro, publíquelos en [!UICONTROL Contenido] y expórtelos para su uso en campañas de marketing.

1. **Para publicar sus nuevas experiencias de correo electrónico**, haga clic en **[!UICONTROL Publicar]** en la barra de herramientas superior o dentro del flujo de aprobaciones.
1. **Para exportar las nuevas experiencias de correo electrónico**, haga clic en **[!UICONTROL Exportar]** en la barra de herramientas superior.
   1. Seleccione el formato (solo CSV e imágenes o HTML) y haga clic en **[!UICONTROL Exportar]**.

Consulte [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) para obtener más información.
