---
title: Editor de código de plantilla
description: Aprenda a utilizar el editor de código de plantilla en GenStudio for Performance Marketing.
level: Intermediate
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
source-git-commit: 19d0b8b929e293179a091cc7b5a6a1268b0abbbd
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

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

### Realice una corrección

Si hay errores en su plantilla, es posible que vea un mensaje de `Template is invalid` que incluye una breve explicación del problema. En el ejemplo siguiente, el mensaje indica que el campo `_image` no se ajusta a la convención de nomenclatura de campos establecida en la plantilla de varios pods. El mensaje también indica que debe actualizar el nombre del campo con el prefijo correcto. Busque el campo `_image` en el editor de código de plantilla y actualice el nombre como se recomienda.

![Corregir plantilla no válida](/help/assets/animation/template-code-editor.gif){width="600" zoomable="yes"}

El panel _[!UICONTROL Comprobar campos detectados]_ se actualiza para reflejar los cambios que ha realizado. Cuando esté seguro de que los campos son correctos y están completos, haga clic en **[!UICONTROL Siguiente]** para continuar [cargando la plantilla](/help/user-guide/content/use-templates.md#add-a-template).
