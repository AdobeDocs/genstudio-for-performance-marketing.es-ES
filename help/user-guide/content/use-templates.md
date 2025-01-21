---
title: Trabajo con plantillas
description: Descubra cómo utilizar las plantillas de forma eficaz para optimizar el proceso creativo en Adobe GenStudio for Performance Marketing.
feature: Templates, Content
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
source-git-commit: 62ab3849296195ca4d9525cb5688f74ce8bede54
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 1%

---

# Trabajo con plantillas

GenStudio for Performance Marketing permite a los creadores de contenido producir rápidamente contenido de marketing coherente de la marca mediante _plantillas_. Una plantilla reduce significativamente el tiempo y el esfuerzo necesarios para generar contenido nuevo al proporcionar un punto de partida que incluye diseños y elementos de diseño preconfigurados.

Aunque GenStudio for Performance Marketing no admite la creación directa de plantillas dentro de la aplicación, puede diseñar y preparar fácilmente plantillas con herramientas de diseño populares, como Adobe InDesign, Illustrator o Express. Una vez completado el diseño, puede adaptarlo para utilizarlo en GenStudio for Performance Marketing. Empiece a utilizar las plantillas siguiendo estos pasos:

1. **Diseña tu plantilla**: usa tu herramienta de diseño preferida para crear el diseño visual de tu [plantilla con elementos](#template-elements) como un preencabezado, un titular, un cuerpo, un CTA, imágenes y un pie de página.

2. **Codifique su plantilla**: convierta su diseño en CSS en línea y de HTML para asegurarse de que esté limpio y adaptable en varios dispositivos. Tenga en cuenta las [directrices de accesibilidad](accessibility-for-templates.md) para alcanzar la audiencia máxima deseada.

3. **Prepararse para GenStudio for Performance Marketing**: adapte la plantilla de HTML mediante el lenguaje de creación de plantillas Handlebars. Inserte marcadores de posición para indicar dónde debe generar contenido GenStudio for Performance Marketing de forma dinámica. Ver cómo [personalizar una plantilla](customize-template.md) para GenStudio for Performance Marketing.

Al seguir estos pasos, puede crear plantillas profesionales y eficaces listas para usar en GenStudio for Performance Marketing, lo que le permite producir contenido de marca de forma rápida y eficaz.

## Elementos de plantilla

Una plantilla es un conjunto de instrucciones definidas con HTML y CSS en línea que pueden utilizarse para generar una experiencia de correo electrónico, anuncio social o anuncio en pantalla. Los elementos de plantilla proporcionan la estructura para la creación de contenido.

A continuación se muestra una lista de los elementos que se utilizan en las plantillas y algunos detalles sobre sus características:

- **Encabezado previo**

   - Actúa como una línea de asunto secundaria en un correo electrónico, mejorando la línea de asunto principal
   - Entre 40 y 50 caracteres
   - Visible en la bandeja de entrada junto al asunto antes de abrir el correo electrónico
   - Se utiliza en plantillas de correo electrónico

- **Encabezado**

   - Sección superior del correo electrónico que ve el destinatario al abrir el correo electrónico
   - Establece el tono y proporciona contexto para el contenido incluido
   - Se utiliza en plantillas de correo electrónico

- **Titular**

   - Primer contenido que ve el destinatario
   - Debería ser convincente para captar interés
   - Se utiliza en plantillas de metadatos

- **Cuerpo**

   - Área de contenido principal donde se transmite el mensaje principal
   - Capaz de incluir texto, imágenes y otros medios
   - Se utiliza en plantillas de correo electrónico y metadatos.

- **CTA**

   - El botón Llamada a la acción utiliza una frase y un vínculo
   - Anima al destinatario a realizar una acción específica, como hacer clic en un vínculo o realizar una compra
   - Se utiliza en plantillas de correo electrónico y metadatos.

- **Imágenes**

   - Aumenta el atractivo visual
   - Dividir texto
   - Apoyar el mensaje
   - Debe ser de alta calidad y llamativo
   - Se utiliza en plantillas de correo electrónico y metadatos.

- **Pie de página**

   - Sección inferior que contiene contenido adicional, como detalles de contacto, vínculos de medios sociales, exenciones de responsabilidad legal y opciones de cancelación de suscripción
   - Se utiliza en plantillas de correo electrónico

- **Superposición de texto**

   - Texto en una imagen
   - Utilice para apoyar y mejorar el titular y el cuerpo
   - Se utiliza en plantillas de metadatos

>[!TIP]
>
>Ver los [nombres de campo reconocidos](customize-template.md#recognized-field-names) que GenStudio for Performance Marketing admite para las plantillas de cada tipo de canal.

## Personalizar plantilla

Usted [personaliza su plantilla](customize-template.md) para usarla en GenStudio for Performance Marketing al insertar marcadores de posición de contenido, o campos, que la inteligencia artificial aplicada generativa usa para insertar contenido. GenStudio for Performance Marketing reconoce ciertos campos, como el campo `body`, y se adhiere a las directrices de canal configuradas para la marca seleccionada.

>[!TIP]
>
>Siga las [directrices de accesibilidad](accessibility-for-templates.md) y las [prácticas recomendadas](/help/user-guide/content/best-practices-for-templates.md) para que pueda llegar a más audiencia y proporcionar una experiencia óptima.

## Administración de plantillas

La galería [!DNL Templates] muestra su inventario de plantillas personalizadas para generar experiencias en GenStudio for Performance Marketing. Puede filtrar las plantillas por tipo de canal, como correo electrónico, anuncios en pantalla y anuncios Meta.

![Lista de plantillas de contenido](/help/assets/content-templates.png){width="650" zoomable="yes"}

### Añadir una plantilla

Antes de cargar una plantilla, asegúrate de que esté totalmente preparada y lista para usarla en GenStudio for Performance Marketing siguiendo las instrucciones de [Personalizar plantillas](customize-template.md).

**Para agregar una plantilla**:

1. En _[!DNL Content]_, seleccione la sección **[!UICONTROL Plantillas]**.

1. Haga clic en **[!UICONTROL Agregar plantilla]**.

1. En el panel _[!UICONTROL Agregar la plantilla aprobada]_, busque el archivo de plantilla de HTML o arrastre el archivo de plantilla de HTML al espacio de colocación. Haga clic en **[!UICONTROL Siguiente]**.

1. En el panel _[!UICONTROL Revisar campos detectados]_, revise los campos detectados. Compruebe que está utilizando la plantilla correcta y que todos los detalles son los esperados. Haga clic en **[!UICONTROL Siguiente]**.

   Ejemplo de previsualización para una plantilla de correo electrónico:

   ![Campos de vista previa detectados](/help/assets/template-detected-fields.png){width="650"}

   >[!TIP]
   >
   >Si la plantilla no es correcta, haga clic en **[!UICONTROL Atrás]** y vuelva al paso anterior. Cargue el archivo de plantilla corregido.

1. En el panel _[!UICONTROL Proporcionar detalles de plantilla y cargar]_, asigne un nombre a la plantilla y seleccione un tipo de **[!UICONTROL canal]**.

   El nombre de la plantilla y el tipo de canal son obligatorios. Los requisitos adicionales pueden incluir:

   - **Meta**: requiere proporción de aspecto
   - **Anuncios de visualización**: requiere Dimension

1. Añada tantos detalles como pueda para mejorar la identificación de la plantilla en las búsquedas y el filtrado.

1. Haga clic en **[!UICONTROL Listo]**.

### Actualizar plantilla

Las plantillas pueden incluir archivos estáticos, como iconos o logotipos. [El contenido estático](/help/user-guide/content/customize-template.md#static-content) no se almacena después de crear la vista previa de la plantilla. GenStudio for Performance Marketing sigue haciendo referencia al vínculo de origen proporcionado en la plantilla. Utilice la actualización para actualizar la vista previa de la plantilla con las últimas versiones de estos recursos.

**Para actualizar la plantilla**:

1. En _[!DNL Content]_, seleccione la sección **[!UICONTROL Plantillas]**.

1. Haga clic en una plantilla para obtener una vista completa y una lista de detalles.

1. Haga clic en **[!UICONTROL Actualizar]** (flechas de círculo) desde la esquina superior derecha para actualizar todos los recursos utilizados en la plantilla.

### Crear una experiencia con una plantilla

Busque y utilice una plantilla existente en GenStudio for Performance Marketing para crear más experiencias.

**Para crear una experiencia con una plantilla**:

1. En _[!DNL Content]_, seleccione la sección **[!UICONTROL Plantillas]**.

1. Haga clic en una plantilla para obtener una vista completa y una lista de detalles.

1. Haga clic en **[!UICONTROL Crear experiencia]** (pincel) en la esquina superior derecha para usar la plantilla.

1. Continuar para [crear](/help/user-guide/create/overview.md#create-use-cases) una experiencia.
