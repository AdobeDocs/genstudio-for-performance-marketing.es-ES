---
title: Editor de código de plantilla
description: Aprenda a utilizar el editor de código de plantilla en GenStudio for Performance Marketing.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
source-git-commit: 81c4b10e22ac347eb2a464496bd65b29c3c94efa
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 1%

---

# Editor de código de plantilla

El editor de código de plantilla está diseñado para ayudarle a comprobar y refinar la plantilla para un uso óptimo al generar nuevas experiencias con GenStudio for Performance Marketing. El editor admite la sintaxis Handlebars, que utiliza marcadores de posición dentro de la plantilla para indicar dónde GenStudio for Performance Marketing debe generar contenido.

>[!TIP]
>
>Antes de cargar el código HTML de la plantilla en la vista [!DNL Content] _Plantillas_, prepare la plantilla insertando los marcadores de posición de contenido definidos en la guía [Personalizar plantillas](customize-template.md).

## Comprobar campos detectados

El panel _[!UICONTROL Comprobar campos detectados]_ muestra una lista de campos que GenStudio for Performance Marketing reconoce en la plantilla. Revise la lista y puede desplazarse por el código HTML para ver la formación de la plantilla.

![Vista del editor de código](/help/assets/template-detected-fields.png "Comprobar campos detectados"){width="600" zoomable="yes"}

Si observa que falta un campo en la lista, busque el código de plantilla y busque la ubicación del campo que falta. Inserte el marcador de posición correcto mediante la sintaxis Handlebars y un [nombre de campo reconocido](/help/user-guide/content/customize-template.md#recognized-field-names). Utilice el formulario Buscar y reemplazar, que aparece en la parte inferior del editor de código, para buscar cadenas específicas en el código. (Windows `CTRL`+`F` o macOS `CMD`+`F`)

## Ajuste de funciones de una variable

Puede seleccionar y cambiar los roles de los campos basados en texto (por ejemplo, `headline`, `sub_headline`, `body`, `cta`, `on_image_text`, `custom`) con un menú desplegable durante la comprobación de la estructura de la plantilla. Las selecciones de funciones de campo persisten durante las ediciones de plantilla para que las personalizaciones no se pierdan, lo que mejora la eficacia del flujo de trabajo.

>[!NOTE]
>
>Las variables de imagen no pueden tener sus funciones ajustadas.

![Selección de campo de varios roles](/help/assets/multirole-dropdown-field.png "Selección de campo de varios roles"){width="600" zoomable="yes"}

Para asignar una función a una variable:

1. Busque la variable en el panel _[!UICONTROL Comprobar campos detectados]_. Estas variables se descubren automáticamente.
2. Revise las funciones asignadas a cada variable. Las funciones se asignan automáticamente, pero se pueden ajustar mediante la lista desplegable de cualquier variable de la plantilla.
3. Para ajustar una función, seleccione una nueva función en la lista desplegable.
4. Haga clic en **[!UICONTROL Siguiente]** para continuar.

## Realice una corrección

Si hay errores en su plantilla, es posible que vea un mensaje de `Template is invalid` que incluye una breve explicación del problema. En el ejemplo siguiente, el mensaje indica que el campo `_image` no se ajusta a la convención de nomenclatura de campos establecida en la plantilla de varios pods. El mensaje también indica que debe actualizar el nombre del campo con el prefijo correcto. Busque el campo `_image` en el editor de código de plantilla y actualice el nombre como se recomienda.

![Corregir plantilla no válida](/help/assets/animation/template-code-editor.gif){width="600" zoomable="yes"}

El panel _[!UICONTROL Comprobar campos detectados]_ se actualiza para reflejar los cambios que ha realizado. Cuando esté seguro de que los campos son correctos y están completos, haga clic en **[!UICONTROL Siguiente]** para continuar [cargando la plantilla](/help/user-guide/content/use-templates.md#add-a-template).

## Problemas y soluciones comunes de las plantillas

| **Error** | **Descripción** | **Solución** |
|-----------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| Error al analizar | No se pudo analizar el contenido de la plantilla como Handlebars válidos. | Compruebe si hay errores de sintaxis de HTML y Handlebars y corríjalos para garantizar un formato válido para [los marcadores de posición de contenido](/help/user-guide/content/customize-template.md#content-placeholders). |
| Grupo no asignado | Un campo de imagen en una plantilla de correo electrónico de varios grupos no está asignado a ningún grupo. | Compruebe si los prefijos de sección se utilizan de forma coherente. Cada [sección](/help/user-guide/content/customize-template.md#sections-or-groups) solo puede usar uno de cada tipo de campo (`headline`, `body`, `image` `cta`). Asigne el campo `image` a un grupo válido de la plantilla. |
| Falta la imagen | Falta un campo de imagen obligatorio. | Se requiere exactamente un campo `image` para ciertos tipos de plantilla, como un anuncio Meta, de visualización o de banner. Agregue el campo `image` requerido a la plantilla. |
| Grupo único no válido | La plantilla de correo electrónico contiene exactamente un grupo, lo que no es válido. | Una plantilla de correo electrónico básica contiene un único conjunto de elementos de plantilla que no requieren la convención de nomenclatura de grupos definida en [Secciones o grupos](/help/user-guide/content/customize-template.md#sections-or-groups). Ajuste la plantilla para que tenga cero secciones quitando cualquier sintaxis de nomenclatura de grupo. |
| Sin campos | La plantilla no contiene ningún campo. | Agregue [nombres de campo reconocidos](/help/user-guide/content/customize-template.md#recognized-field-names) mediante la sintaxis Handlebars a la plantilla donde necesita que GenStudio for Performance Marketing genere un determinado tipo de contenido. |
| Faltan propiedades requeridas | Faltan algunas propiedades de metadatos requeridas. | Cada tipo de plantilla tiene requisitos y restricciones basados en las directrices de canal. Por ejemplo, Meta requiere una proporción de aspecto y los anuncios de visualización requieren dimensiones. [Siga las directrices de plantillas específicas del canal](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines). |
| Nombre reservado utilizado | Se está utilizando un nombre de campo prohibido o reservado. | Algunos [nombres de campo](/help/user-guide/content/customize-template.md#recognized-field-names), como `subject` o `introductory_text`, están reservados. Cambie el nombre de los campos que utilizan nombres reservados o prohibidos. |
| Demasiados campos | El número de campos supera el límite global de 20. | Elimine los campos innecesarios para asegurarse de que el total no supera los 20. |
| Demasiados grupos | El número de grupos supera el máximo permitido del canal. | Las plantillas meta, display y LinkedIn no permiten varias secciones. El correo electrónico requiere un nombre de grupo al definir dos o tres secciones. Reduzca la cantidad de grupos en su plantilla para cumplir con los [requisitos del canal](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines). |
| Campo no compatible | La plantilla utiliza un campo que el canal no admite. | Reemplazar o quitar campos no admitidos según los [nombres de campo reconocidos](/help/user-guide/content/customize-template.md#recognized-field-names). |
