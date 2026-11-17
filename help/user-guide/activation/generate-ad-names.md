---
title: Generar nombres de anuncios
description: Obtenga información sobre cómo configurar plantillas de nombres, generar nombres de anuncios coherentes y revisar o personalizar nombres antes de enviar anuncios a las plataformas de activación admitidas.
role: User
source-git-commit: 7863995df08681a8a427277121a5fbeca131c6a9
workflow-type: tm+mt
source-wordcount: '1575'
ht-degree: 1%
---

# Generar nombres de anuncios

La asignación automatizada de nombres a los anuncios en [!DNL GenStudio for Performance Marketing] le ayuda a seguir las convenciones de asignación de nombres de su organización cuando activa los anuncios. Los nombres coherentes admiten la creación de informes de rendimiento, la atribución y la reconciliación de gastos.

Cargue la convención de nombres para crear una plantilla y úsela para generar nombres a partir de metadatos de experiencia. Revise los resultados y realice las correcciones necesarias antes de enviar anuncios a sus plataformas.

## Antes de empezar

La configuración de plantillas es una tarea de una sola vez. Si su plataforma ya tiene una plantilla asignada en su proyecto actual, vaya a [Generar nombres para una activación](#generate-names-for-an-activation).

Para configurar la plantilla, prepare un archivo de Excel de no más de 3 MB con una sola hoja. No se admiten archivos CSV. Describa la convención de nombres para anuncios individuales, no para campañas o grupos de anuncios.

Incluya los campos en el orden requerido, los valores permitidos, los códigos correspondientes e instrucciones para elegir valores. Por ejemplo, si se selecciona `Image` para el campo `format`, se puede producir `IMG` en el nombre.

Descargue el [ejemplo de convención de nomenclatura WKND Meta (Excel)](assets/wknd-meta-naming-convention.xlsx) para explorar una estructura de muestra. Incluye definiciones de campo y valores de ejemplo para año, trimestre, marca, producto, campaña, plataforma, formato, versión creativa, persona, mercado, idioma y CTA.

Reemplace los valores y las reglas de ejemplo por la convención de su organización antes de utilizar el archivo para sus propias activaciones. Los valores de plataforma del ejemplo ilustran las opciones de nomenclatura, no una lista de destinos de activación admitidos.

Un administrador del sistema debe asignar la plantilla a sus plataformas. Los distintos proyectos pueden utilizar diferentes plantillas predeterminadas para la misma plataforma.

## Creación de una plantilla de nomenclatura

Cree una plantilla a partir del archivo de convención de nombres existente y, a continuación, revise la estructura extraída antes de utilizarla.

1. Abra el proyecto en el que desee utilizar la plantilla.
1. Vaya a **[!UICONTROL Más]** > **[!UICONTROL Configuración]**.
1. Seleccione **[!UICONTROL Configurar]** junto a **[!UICONTROL Plantilla de nombre de anuncio]**.

   Si las plantillas ya existen, abre **[!UICONTROL Plantilla de nombre de anuncio]** y luego selecciona **[!UICONTROL Crear plantilla]**.

1. Seleccione **[!UICONTROL Seleccionar archivo]** en el cuadro de diálogo **[!UICONTROL Cargar archivo]**.
1. Elija el archivo de Excel.

   También puede arrastrar el archivo al área de carga. Mientras aparece **[!UICONTROL Analizando la hoja de cálculo...]**, los campos y valores se asignan a la plantilla. Esto puede tardar unos minutos.

1. Revise los campos, los valores permitidos y la **[!UICONTROL vista previa del nombre del anuncio]**.

   La vista previa utiliza valores de muestra, no los detalles de un anuncio específico.

1. Seleccione **[!UICONTROL Guardar]**.

Los archivos de más de 3 MB, los tipos de archivo no compatibles y los archivos vacíos muestran un error sin cambiar las plantillas o asignaciones de plataforma existentes.

## Personalizar una plantilla

Edite una plantilla guardada para ajustar su nombre, campos, separador o reglas.

1. Vaya a **[!UICONTROL Más]** > **[!UICONTROL Configuración]** > **[!UICONTROL Plantilla de nombre de anuncio]**.
1. Abra el menú de tres puntos junto a la plantilla.
1. Seleccione **[!UICONTROL Editar]**.
1. Seleccione el icono de lápiz junto al título para cambiar el nombre de la plantilla.
1. Establezca el **[!UICONTROL separador de campos]** para que coincida con su convención.
1. Arrastre los campos al orden requerido.

   Use **[!UICONTROL Agregar campo]** o el icono de papelera de un campo si necesita cambiar qué campos se incluyen.

1. Seleccione el icono de lápiz de un campo para abrir su configuración.
1. Revise **[!UICONTROL Type]** y **[!UICONTROL Name]** en el cuadro de diálogo **[!UICONTROL Editar un campo]**.

   Use **[!UICONTROL Lista desplegable]** para un campo con opciones predefinidas o **[!UICONTROL Texto libre]** para un valor que usted ingrese.

1. Para ver un campo desplegable, revisa **[!UICONTROL Opciones]** y **[!UICONTROL Código]**.

   **[!UICONTROL Opciones]** contiene las opciones legibles. **[!UICONTROL Code]** contiene los valores correspondientes utilizados en el nombre del anuncio. Por ejemplo, la opción `Image` usa el código `IMG`.

   Use **[!UICONTROL Agregar opción]** para agregar una opción o el icono menos situado junto a una opción para quitarla. No se permiten valores duplicados dentro de un campo.

1. Escriba las **[!UICONTROL reglas de campo]** necesarias para elegir o dar formato al valor de ese campo.

   En el campo de texto libre `creativeVersion` del ejemplo, puede escribir `Use the experience name as a starting value, with spaces removed.`

1. Seleccione **[!UICONTROL Guardar]** en el cuadro de diálogo de campo.

   Repita la revisión de campos para cualquier otro campo que necesite cambios.

1. Escriba **[!UICONTROL reglas de plantilla]** que se apliquen a todo el nombre.

   Por ejemplo, escriba `Remove spaces from Product and Campaign values.`

1. Seleccione **[!UICONTROL Guardar]** en la parte superior de la página.

La vista previa refleja el orden de campos y el separador actualizados. Vuelva a abrir la plantilla para comprobar los cambios guardados.

El editor de campos muestra cómo las opciones legibles se asignan a los códigos incluidos en los nombres generados:

![Editar un cuadro de diálogo de campo con las opciones de formato Imagen, Vídeo, Carrusel y HTML5 y sus códigos correspondientes.](images/ad-name-field-options-codes.png)

## Asignación de una plantilla a las plataformas

Los administradores de sistemas establecen la plantilla predeterminada para cada plataforma dentro de un proyecto. Si no es administrador del sistema, pida a uno que complete este procedimiento.

1. Abra el proyecto cuya plataforma predeterminada desee establecer.
1. Vaya a **[!UICONTROL Más]** > **[!UICONTROL Configuración]** > **[!UICONTROL Plantilla de nombre de anuncio]**.
1. Abra el menú de tres puntos junto a la plantilla.
1. Seleccione **[!UICONTROL Editar]**.
1. Seleccione una o más plataformas en **[!UICONTROL Plataformas preferidas]** en la parte inferior del editor.
1. Seleccione **[!UICONTROL Guardar]**.

Cada plataforma tiene una plantilla predeterminada por proyecto. Puede asignar la misma plantilla a varias plataformas.

Puede ver y editar las plantillas en todos los proyectos, pero sólo puede cambiar las asignaciones del proyecto en el que se encuentra actualmente.

Reemplazar la plantilla predeterminada de una plataforma no elimina la plantilla anterior ni cambia las asignaciones de otros proyectos.

El ejemplo siguiente muestra la vista previa de la plantilla, el orden de los campos, las reglas y las **[!UICONTROL plataformas preferidas]** con Meta Ads seleccionado:

![Editor de plantillas WKND con un separador de guiones bajos, 12 campos con nombre de anuncio, reglas de plantilla y Meta Ads seleccionados en Plataformas preferidas.](images/ad-name-template-editor.png)

## Generación de nombres para una activación

Genere nombres después de preparar la activación y revise los metadatos de experiencia que necesita la plantilla, como campaña, producto o persona.

1. Abra **[!UICONTROL Activar]** en el proyecto deseado.
1. Añada sus experiencias a una activación.
1. Complete la configuración de la plataforma y toda la información necesaria, incluida la copia, call-to-action (CTA) y la dirección URL del sitio web.
1. Compruebe que las experiencias tengan los metadatos necesarios para la convención de nomenclatura.
1. Seleccione **[!UICONTROL Generar nombre de anuncio]** sobre la tabla de activación.

   Espere a que **[!UICONTROL finalice la generación de nombres de anuncios]** antes de revisar los resultados.

1. Revise la columna **[!UICONTROL Nombre del anuncio]**.

La generación se aplica a todos los anuncios de plataformas con una plantilla asignada, excepto a los anuncios con las anulaciones habilitadas. Los nombres no se generan automáticamente al abrir la tabla.

Inicialmente, cada anuncio utiliza el nombre de su experiencia. Si una plataforma no tiene ninguna plantilla asignada, la generación deja sus nombres sin cambiar y puede editarlos manualmente.

Si ninguna plataforma tiene plantillas asignadas, no se genera ningún nombre.

## Corregir un nombre de anuncio individual

Revise los nombres generados antes de enviar sus anuncios. Los valores que faltan aparecen como marcadores de posición de campo resaltados, como `[market]`, y los anuncios afectados muestran **[!UICONTROL Necesita atención]**.

La tabla de activación marca los nombres con valores que faltan para que pueda encontrarlos y corregirlos:

![Tabla de activación con una advertencia de valores ausentes, marcadores de posición de mercado resaltados en la columna Nombre del anuncio y estados de atención necesarios.](images/ad-names-missing-values.png)

1. Seleccione la fila del anuncio en la tabla de activación.
1. Seleccione **[!UICONTROL Editar nombre del anuncio]**.
1. Actualice los campos de texto o desplegables relevantes.
1. Seleccione **[!UICONTROL Guardar]**.

Por ejemplo, si `market` no tiene ningún valor, escriba o seleccione el mercado apropiado para reemplazar a `[market]` en el nombre.

Compruebe el nombre actualizado en relación con la convención.

## Resolver posibles nombres duplicados

Los nombres de anuncios idénticos en la misma plataforma se marcan como posibles duplicados.

1. Seleccione uno de los anuncios afectados.
1. Seleccione **[!UICONTROL Editar nombre del anuncio]**.
1. Cambie el nombre para que los dos nombres sean diferentes.
1. Seleccione **[!UICONTROL Guardar]**.

La advertencia de posible duplicado se borra después de que los nombres se hayan cambiado de nombre.

## Editar varios nombres de anuncio a la vez

Utilice la edición masiva para aplicar una corrección compartida sin reemplazar valores que deban ser diferentes para cada anuncio.

1. Seleccione los anuncios utilizando sus casillas de verificación de fila.
1. Seleccione **[!UICONTROL Editar nombre del anuncio]** en la barra de herramientas de selección.
1. Cambie solo los campos que deben tener el mismo valor en los anuncios seleccionados.

   **[!UICONTROL Valores mixtos]** significa que los anuncios seleccionados tienen actualmente valores diferentes para un campo. Deje ese campo intacto para conservar el valor de cada anuncio.

1. Seleccione **[!UICONTROL Guardar]**.
1. Revise los nombres actualizados para comprobar su precisión y los posibles duplicados.

Solo se actualizan los anuncios seleccionados. Los anuncios no seleccionados permanecen inalterados.

El editor en masa muestra **[!UICONTROL Valores mixtos]** para campos que difieren entre los anuncios seleccionados:

![Detalle del cuadro de diálogo Editar 4 nombres de anuncios que muestra valores mixtos de producto, campaña, creativeVersion y persona.](images/ad-names-bulk-edit.png)

Por ejemplo, si se cambia solamente la persona de `OutdoorBeginners` a `Adventurers`, se conservarán los distintos productos. Estos nombres abreviados ilustran el cambio:

| Antes | Después |
| --- | --- |
| `WKND_TrailBag_OutdoorBeginners` | `WKND_TrailBag_Adventurers` |
| `WKND_RiosShirt_OutdoorBeginners` | `WKND_RiosShirt_Adventurers` |

## Usar un nombre de anuncio personalizado

Anule un nombre generado cuando un anuncio necesite un nombre personalizado completo.

1. Seleccione la fila del anuncio.
1. Seleccione **[!UICONTROL Editar nombre del anuncio]**.
1. Activar **[!UICONTROL Anular nombres de anuncios]**.
1. Introduzca el nombre personalizado.
1. Seleccione **[!UICONTROL Guardar]**.

El nombre personalizado permanece sin cambios cuando se vuelven a generar nombres.

Con la anulación habilitada, puede editar el nombre completo en lugar de sus campos de plantilla individuales:

![Cuadro de diálogo Editar nombre de anuncio con la opción Anular nombres de anuncio habilitada y el nombre completo del anuncio WKND disponible para edición.](images/ad-name-override.png)

Para volver a la nomenclatura basada en plantillas, siga estos pasos:

1. Abra **[!UICONTROL Editar nombre del anuncio]** para el anuncio.
1. Desactivar **[!UICONTROL Anular nombres de anuncios]**.
1. Seleccione **[!UICONTROL Guardar]**.
1. Seleccione **[!UICONTROL Generar nombre de anuncio]** sobre la tabla de activación.

Esta acción de generación también se aplica a los demás anuncios aptos de la tabla.

## Responder a los cambios de plantilla

Al editar una tabla de activación, aparece una advertencia si una plantilla que utiliza ha cambiado o se ha eliminado.

Si la plantilla ha cambiado, revise la plantilla actualizada antes de volver a generar los nombres. Seleccione **[!UICONTROL Generar nombre de anuncio]** para aplicarlo.

Si la plantilla se ha eliminado o necesita un reemplazo, siga estos pasos:

1. Pida a un administrador del sistema que asigne una plantilla de reemplazo a la plataforma afectada en el mismo proyecto.
1. Vuelva a la tabla de activación.
1. Seleccione **[!UICONTROL Generar nombre de anuncio]**.
1. Revise los nombres actualizados.

Los nombres con las sustituciones activadas permanecen inalterados durante la regeneración.

## Envío de anuncios a las plataformas

Revisa los nombres y direcciones finales de los campos no resueltos, posibles duplicados y otros **[!UICONTROL problemas que requieren atención]** antes de enviar anuncios.

Cuando la activación esté lista, seleccione **[!UICONTROL Enviar a plataformas]**.

Los nombres publicados coinciden exactamente con los nombres finales de [!DNL GenStudio for Performance Marketing], incluidos los nombres generados, los nombres editados mediante campos de plantilla y los nombres reemplazados.

Para destinos de visualización como Innovid, los nombres aparecen como nombres creativos.
