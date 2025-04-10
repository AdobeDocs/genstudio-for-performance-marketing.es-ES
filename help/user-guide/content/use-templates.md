---
title: Trabajo con plantillas
description: Descubra cómo utilizar las plantillas de forma eficaz para optimizar el proceso creativo en Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer
feature: Media Templates
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
source-git-commit: 1f62546f4fc2381bcc4d8fd3acadd1d6470ed9e8
workflow-type: tm+mt
source-wordcount: '1326'
ht-degree: 1%

---

# Trabajo con plantillas

GenStudio for Performance Marketing permite a los creadores de contenido producir rápidamente contenido de marketing coherente de la marca mediante _plantillas_. Una plantilla reduce significativamente el tiempo y el esfuerzo necesarios para generar contenido nuevo al proporcionar un punto de partida que incluye diseños y elementos de diseño preconfigurados.

Aunque GenStudio for Performance Marketing no admite la creación directa de plantillas dentro de la aplicación, puede diseñar y preparar fácilmente plantillas con herramientas de diseño populares, como Adobe InDesign, Illustrator o Express. Una vez completado el diseño, puede adaptarlo para utilizarlo en GenStudio for Performance Marketing. Empiece a utilizar las plantillas siguiendo estos pasos:

1. **Diseña tu plantilla**: usa tu herramienta de diseño preferida para crear el diseño visual de tu [plantilla con elementos](#template-elements) como un preencabezado, un titular, un cuerpo, un CTA, imágenes y un pie de página.

2. **Codifique su plantilla**: convierta su diseño en HTML y CSS en línea para asegurarse de que esté limpio y adaptable en varios dispositivos. Tenga en cuenta las [directrices de accesibilidad](accessibility-for-templates.md) para alcanzar la audiencia máxima deseada.

3. **Prepararse para GenStudio for Performance Marketing**: adapte la plantilla de HTML usando el lenguaje de creación de plantillas Handlebars. Inserte marcadores de posición para indicar dónde debe generar contenido GenStudio for Performance Marketing de forma dinámica. Ver cómo [personalizar una plantilla](customize-template.md) para GenStudio for Performance Marketing.

Al seguir estos pasos, puede crear plantillas profesionales y eficaces listas para usar en GenStudio for Performance Marketing, lo que le permite producir contenido de marca de forma rápida y eficaz.

## Elementos de plantilla

Una plantilla es un conjunto de instrucciones definidas con HTML y CSS en línea que puede utilizarse para generar una experiencia de correo electrónico, anuncio social o anuncio en pantalla. Los elementos de plantilla proporcionan la estructura para la creación de contenido.

A continuación se muestra una lista de los elementos que se utilizan en las plantillas y algunos detalles sobre sus características:

| **Elemento** | **Canal** | **Descripción** |
|----------------------|------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Encabezado previo** | Correo electrónico | Una línea de asunto secundaria en un correo electrónico, normalmente entre 40 y 50 caracteres, que mejora la línea de asunto principal. Se puede ver en la bandeja de entrada junto al asunto antes de abrir el correo electrónico. |
| **Encabezado** | Correo electrónico | La sección superior del correo electrónico que ve el destinatario al abrir el correo electrónico establece el tono y proporciona contexto para el contenido incluido. |
| **Titular** | Meta ad, Banner y anuncios de visualización, LinkedIn | El primer contenido que el destinatario ve debe ser convincente para captar el interés. |
| **Subtítulo** | Correo electrónico, banner y anuncios en pantalla | Elemento de texto secundario que admite el titular. Por lo general, es conciso y está diseñado para complementar el titular principal, lo que lleva la atención del lector más allá en el contenido. |
| **Texto introductorio** | LinkedIn | El mensaje principal transmite el mensaje principal, similar a la copia de cuerpo. Puede utilizar hasta 150 caracteres, incluidos espacios, un máximo de cuatro emojis y puntuación. |
| **Cuerpo** | Correo electrónico, Meta-anuncio, Banner y Anuncios en pantalla | El texto principal del anuncio transmite el mensaje principal. Debe ser atractivo, informativo y persuasivo alentar la acción deseada de la audiencia. |
| **CTA** | Correo electrónico, publicidad en metadatos, anuncios en banners y pantallas, LinkedIn | Un botón de call-to-action utiliza una frase y un vínculo para animar al destinatario a realizar una acción específica, como hacer clic en un vínculo o realizar una compra. |
| **Imágenes** | Correo electrónico, publicidad en metadatos, anuncios en banners y pantallas, LinkedIn | Mejore el atractivo visual, divida el texto y admita el mensaje. Las imágenes deben ser de alta calidad y llamativas. |
| **Pie de página** | Correo electrónico | La sección inferior del correo electrónico contiene contenido adicional, como detalles de contacto, vínculos de medios sociales, exenciones de responsabilidad y opciones de cancelación de suscripción. |
| **Superposición de texto** | Meta anuncio | Texto colocado en una imagen para apoyar y mejorar el titular y el contenido del cuerpo. |

>[!TIP]
>
>Ver los [nombres de campo reconocidos](customize-template.md#recognized-field-names) que GenStudio for Performance Marketing admite para las plantillas de cada tipo de canal.

## Personalizar plantilla

Usted [personaliza su plantilla](customize-template.md) para usarla en GenStudio for Performance Marketing al insertar marcadores de posición de contenido, o campos, que la inteligencia artificial aplicada generativa usa para insertar contenido. GenStudio for Performance Marketing reconoce ciertos campos, como el campo `body`, y se adhiere a las directrices de canal configuradas para la marca seleccionada.

>[!TIP]
>
>Siga las [directrices de accesibilidad](accessibility-for-templates.md) y las [prácticas recomendadas](/help/user-guide/content/best-practices-for-templates.md) para que pueda llegar a más audiencia y proporcionar una experiencia óptima.

## Administración de plantillas

La galería _[!DNL Templates]_muestra su inventario de plantillas personalizadas para generar experiencias en GenStudio for Performance Marketing.

### Buscar conjunto de datos

Cada vista de [!DNL Content] proporciona opciones de filtro para restringir la búsqueda del recurso, la experiencia o la plantilla ideales. Hay filtros basados en [directrices](/help/user-guide/guidelines/overview.md), [palabras clave](asset-details.md#user-defined-metadata) y [categorías de atributos](/help/user-guide/insights/attributes.md#categories) para reducir los resultados de búsqueda.

Por ejemplo, es posible que desee encontrar una plantilla con un tipo de canal o una proporción de aspecto específicos creados por usted:

- **[!UICONTROL Creado por]**: limita la lista _[!UICONTROL Plantillas]_ para mostrar únicamente las plantillas creadas por usted o por una persona específica.
- **[!UICONTROL Proporción de aspecto]**: limita la lista _[!UICONTROL Plantillas]_ para mostrar plantillas diseñadas para una proporción de aspecto específica.

A continuación, se muestra un filtro por tipo de canal, como correo electrónico, anuncios de visualización, anuncios Meta y anuncios LinkedIn.

![Lista de plantillas de contenido](/help/assets/content-templates-filter.png "Buscar en las plantillas de LinkedIn"){width="650" zoomable="yes"}

La capacidad de búsqueda de plantillas está disponible durante [!UICONTROL Crear] al seleccionar una plantilla para medios propios o de pago. Si determinadas opciones de filtro no están visibles, indica que ninguna plantilla del repositorio coincide con los criterios de metadatos correspondientes. Asegúrese de que las plantillas estén etiquetadas correctamente con los metadatos para que se puedan detectar a través de estos filtros.

### Añadir una plantilla

Antes de cargar una plantilla, asegúrate de que esté totalmente preparada y lista para usarla en GenStudio for Performance Marketing siguiendo las instrucciones que se indican en [Personalizar plantillas](customize-template.md).

**Para agregar una plantilla**:

1. En _[!DNL Content]_, seleccione la sección **[!UICONTROL Plantillas]**.

1. Haga clic en **[!UICONTROL Agregar plantilla]**.

1. En el panel _[!UICONTROL Agregar su plantilla aprobada]_, busque el archivo de plantilla de HTML o arrastre el archivo de plantilla de HTML al espacio de colocación. Haga clic en **[!UICONTROL Siguiente]**.

1. En el panel _[!UICONTROL Comprobar campos detectados]_, revise los campos. Compruebe que está utilizando la plantilla correcta y que todos los detalles son los esperados.

   Ejemplo de previsualización para una plantilla de correo electrónico:

   ![Campos de vista previa detectados](/help/assets/template-detected-fields.png){width="650" zoomable="yes"}

   >[!TIP]
   >
   >Si la plantilla no es correcta, haga clic en **[!UICONTROL Atrás]** y vuelva al paso anterior. Cargue el archivo de plantilla corregido. O use el [editor de código de plantilla](/help/user-guide/content/code-editor.md) para hacer correcciones simples.

1. Haga clic en **[!UICONTROL Siguiente]** cuando esté satisfecho con la vista previa de la plantilla.

1. En _[!UICONTROL Proporcione detalles de plantilla y cargue]_, asigne un nombre a la plantilla y seleccione un tipo de **[!UICONTROL canal]**.

   El nombre de la plantilla y el tipo de canal son obligatorios. Los requisitos adicionales pueden incluir:

   - **Meta**: requiere proporción de aspecto
   - **Titular y anuncio para mostrar**: requiere dimensiones

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

## Plantillas de AJO y Marketo

Puede cargar una plantilla que haya creado en Adobe Journey Optimizer (AJO) o Marketo. GenStudio for Performance Marketing detecta los patrones específicos de la aplicación y los ignora, conservando el formulario original para utilizarlo de forma continua en AJO o Marketo. No es necesario realizar ningún cambio en la sintaxis original de AJO o Marketo.

Los patrones de aplicación reconocidos incluyen:

- **AJO**: `{{profile.*}}`, `{{context.*}}`
- **Marketo**: `{{my.*}}`, `{{lead.*}}`, `{{system.*}}`

>[!BEGINSHADEBOX]

**Requisitos previos**

- La aplicación (AJO, Marketo) y GenStudio for Performance Marketing deben pertenecer a la misma organización de IMS para la integración
- Los usuarios deben tener la función &quot;Colaborador&quot; (nivel inferior) o superior

>[!ENDSHADEBOX]

A continuación, [personalice su plantilla](/help/user-guide/content/customize-template.md) con marcadores de posición para indicar dónde GenStudio for Performance Marketing debe generarle contenido. [Agregue su plantilla](#add-a-template) al repositorio [!DNL Content] y valide la plantilla. Realice correcciones menores con el editor de código.
