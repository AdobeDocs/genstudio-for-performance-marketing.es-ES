---
title: Generar nombres de anuncios
description: Obtenga información sobre cómo configurar plantillas de nombres, generar nombres de anuncios coherentes y revisar o personalizar nombres antes de enviar anuncios a las plataformas de activación admitidas.
role: User
source-git-commit: 888a9509ed1c3705f67fbf541b38a49b7890ac7d
workflow-type: tm+mt
source-wordcount: '1746'
ht-degree: 1%
---

# Generar nombres de anuncios

La asignación automatizada de nombres a los anuncios en [!DNL GenStudio for Performance Marketing] le ayuda a seguir las convenciones de asignación de nombres de su organización cuando activa los anuncios. Los nombres coherentes admiten la creación de informes de rendimiento, la atribución y la reconciliación de gastos.

Una plantilla de nomenclatura define las partes del nombre de un anuncio y su orden. Algunas partes de ejemplo son el producto, la campaña y el mercado. Para crear una plantilla, cargue un archivo de Excel que describa la convención de nombres de su organización.

Utilice la plantilla para generar nombres a partir de información sobre cada experiencia, como su producto o campaña. Revise y corrija los resultados antes de enviar sus anuncios. Los nombres finales se envían a cada plataforma de destino como los nombres de los anuncios.

## Antes de empezar

Solo es necesario configurar una plantilla una vez. Si su plataforma ya tiene una plantilla asignada en su proyecto actual, vaya directamente a [Generar nombres para una activación](#generate-names-for-an-activation).

De lo contrario, cree una plantilla y pídale al administrador del sistema que [la asigne a sus plataformas](#assign-a-template-to-platforms). Cada proyecto puede tener una plantilla predeterminada diferente para la misma plataforma.

Para configurar la plantilla, prepare un archivo de Excel de no más de 3 MB con una sola hoja. No se admiten archivos CSV. Describa la convención de nombres para anuncios individuales, no para campañas o grupos de anuncios.

Enumere los campos en el orden requerido. Para cada campo, incluya los valores permitidos, los códigos correspondientes e instrucciones para elegir un valor. Por ejemplo, la opción `Image` del campo `format` utiliza el código `IMG` en el nombre.

Para obtener una estructura de ejemplo, descargue el [ejemplo de convención de nombres de WKND Meta (Excel)](assets/wknd-meta-naming-convention.xlsx). El archivo define campos y valores de ejemplo para productos, campañas, mercados y otras partes del nombre de un anuncio.

Reemplace los valores y las reglas de ejemplo por la convención de su organización antes de utilizar el archivo para sus propias activaciones. Los valores de plataforma del ejemplo ilustran las opciones de nomenclatura, no una lista de destinos de activación admitidos.

## Creación de una plantilla de nomenclatura

Cree una plantilla a partir del archivo de convención de nombres existente y, a continuación, revise la estructura extraída antes de utilizarla.

1. Abra el proyecto en el que desee utilizar la plantilla.
1. Vaya a **[!UICONTROL Más]** > **[!UICONTROL Configuración]**.
1. Seleccione **[!UICONTROL Configurar]** junto a **[!UICONTROL Plantilla de nombre de anuncio]**.

   Si las plantillas ya existen, abre **[!UICONTROL Plantilla de nombre de anuncio]** y luego selecciona **[!UICONTROL Crear plantilla]**.

1. Seleccione **[!UICONTROL Seleccionar archivo]** en el cuadro de diálogo **[!UICONTROL Cargar archivo]**.
1. Elija el archivo de Excel.

   También puede arrastrar el archivo al área de carga. Mientras aparece **[!UICONTROL Analizando la hoja de cálculo...]**, los campos y valores se asignan a la plantilla. Espere unos minutos para que finalice el análisis.

1. Revise los campos, los valores permitidos y la **[!UICONTROL vista previa del nombre del anuncio]**.

   La vista previa utiliza valores de muestra, no los detalles de un anuncio específico.

1. Seleccione **[!UICONTROL Guardar]**.

Los archivos de más de 3 MB, los tipos de archivo no compatibles y los archivos vacíos muestran un error sin cambiar las plantillas o asignaciones de plataforma existentes.

## Personalizar una plantilla

Edite una plantilla guardada para ajustar su nombre, campos, separador o reglas.

1. Vaya a **[!UICONTROL Más]** > **[!UICONTROL Configuración]** > **[!UICONTROL Plantilla de nombre de anuncio]**.
1. Abra el menú de tres puntos junto a la plantilla.
1. Seleccione **[!UICONTROL Editar]**.
1. Para cambiar el nombre de la plantilla, seleccione el icono de lápiz junto al título.
1. Establezca el **[!UICONTROL separador de campos]** en el carácter que separa las partes del nombre, como un guion bajo (`_`).
1. Arrastre los campos al orden requerido.

   Use **[!UICONTROL Agregar campo]** o el icono de papelera de un campo si necesita cambiar qué campos se incluyen.

1. Para abrir la configuración de un campo, seleccione su icono de lápiz.
1. Revise **[!UICONTROL Type]** y **[!UICONTROL Name]** en el cuadro de diálogo **[!UICONTROL Editar un campo]**.

   Use **[!UICONTROL Lista desplegable]** para un campo con opciones predefinidas o **[!UICONTROL Texto libre]** para un valor que usted ingrese.

1. Para ver un campo desplegable, revisa **[!UICONTROL Opciones]** y **[!UICONTROL Código]**.

   **[!UICONTROL Opciones]** contiene las opciones legibles. **[!UICONTROL Code]** contiene los valores correspondientes utilizados en el nombre del anuncio. Por ejemplo, la opción `Image` usa el código `IMG`.

   Para agregar una opción, seleccione **[!UICONTROL Agregar opción]**. Para eliminar una opción, seleccione su icono menos. No se permiten valores duplicados dentro de un campo.

1. Escriba las **[!UICONTROL reglas de campo]** necesarias para elegir o dar formato al valor de ese campo.

   Para el campo de texto libre `creativeVersion`, escriba esta regla de ejemplo: `Use the experience name as a starting value, with spaces removed.`

1. Seleccione **[!UICONTROL Guardar]** en el cuadro de diálogo de campo.

   Repita la revisión de campos para cualquier otro campo que necesite cambios.

1. Escriba **[!UICONTROL reglas de plantilla]** que se apliquen a todo el nombre.

   Por ejemplo, escriba `Remove spaces from Product and Campaign values.`

1. Seleccione **[!UICONTROL Guardar]** en la parte superior de la página.

La vista previa refleja el orden de campos y el separador actualizados. Para comprobar los cambios guardados, vuelva a abrir la plantilla.

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

Las plantillas están disponibles para su visualización y edición en todos los proyectos. Sin embargo, sólo puede cambiar las asignaciones de la plataforma en el proyecto actual.

Reemplazar la plantilla predeterminada de una plataforma no elimina la plantilla anterior ni cambia las asignaciones de otros proyectos.

El ejemplo siguiente muestra la vista previa de la plantilla, el orden de los campos, las reglas y las **[!UICONTROL plataformas preferidas]** con Meta Ads seleccionado:

![Editor de plantillas WKND con un separador de guiones bajos, 12 campos con nombre de anuncio, reglas de plantilla y Meta Ads seleccionados en Plataformas preferidas.](images/ad-name-template-editor.png)

## Generación de nombres para una activación

Prepare la activación antes de generar los nombres. Los metadatos de cada experiencia contienen información como su campaña, producto o persona. Compruebe que los metadatos proporcionan los valores que necesita la plantilla. Consulte [Flujo de trabajo de activación](create-activation.md) para obtener ayuda con la preparación de una activación.

Cuando crea una activación por primera vez, el nombre inicial de cada anuncio depende de la asignación de plantilla de su plataforma:

| Configuración de plataforma | Nombre del anuncio inicial |
| --- | --- |
| Se asigna una plantilla de nombre al proyecto actual. | Los campos de plantilla vacíos aparecen como marcadores de posición, como `[market]_[year]`. Los nombres solo se generan después de seleccionar **[!UICONTROL Generar nombre de anuncio]**. |
| No se ha asignado ninguna plantilla de nombre al proyecto actual. | El anuncio utiliza el nombre de su experiencia. La generación de nombres deja ese nombre sin cambios. |

1. Abra **[!UICONTROL Activar]** en el proyecto deseado.
1. Añada sus experiencias a una activación.
1. Complete la configuración de la plataforma y toda la información necesaria, incluida la copia, call-to-action (CTA) y la dirección URL del sitio web.
1. Compruebe que las experiencias tengan los metadatos necesarios para la convención de nomenclatura.
1. Seleccione **[!UICONTROL Generar nombre de anuncio]** sobre la tabla de activación.

   Espere a que **[!UICONTROL finalice la generación de nombres de anuncios]** antes de revisar los resultados.

1. Revise la columna **[!UICONTROL Nombre del anuncio]**.

La generación se aplica a todos los anuncios de plataformas con una plantilla asignada, excepto a los anuncios con [invalidaciones de nombres personalizados](#use-a-custom-ad-name). Los nombres no se generan automáticamente al abrir la tabla.

Para plataformas sin una plantilla asignada, edite los nombres de los anuncios basados en la experiencia manualmente según sea necesario.

Si ninguna plataforma tiene plantillas asignadas, no se genera ningún nombre.

## Corregir un nombre de anuncio individual

Revise los nombres generados antes de enviar sus anuncios. Cualquier campo que permanezca vacío después de la generación aparecerá como marcador resaltado, como `[market]`. Los anuncios afectados muestran **[!UICONTROL Necesita atención]**.

Para buscar nombres que necesiten correcciones, busque marcadores de posición resaltados y **[!UICONTROL Necesita atención]** estados en la tabla de activación:

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

## Editar varios nombres de publicidad {#edit-several-ad-names-at-once}

Utilice la edición masiva para aplicar una corrección compartida, conservando al mismo tiempo los valores que difieren entre anuncios.

1. Seleccione los anuncios utilizando sus casillas de verificación de fila.
1. Seleccione **[!UICONTROL Editar nombre del anuncio]** en la barra de herramientas de selección.
1. Cambie solo los campos que necesiten el mismo valor en los anuncios seleccionados.

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

Utilice una anulación para reemplazar todo el nombre generado con un nombre personalizado, en lugar de editar campos de plantilla individuales.

1. Seleccione la fila del anuncio.
1. Seleccione **[!UICONTROL Editar nombre del anuncio]**.
1. Activar **[!UICONTROL Anular nombres de anuncios]**.
1. Introduzca el nombre personalizado.
1. Seleccione **[!UICONTROL Guardar]**.

El nombre personalizado permanece sin cambios cuando se vuelven a generar nombres.

Con la anulación habilitada, edite el nombre completo en lugar de sus campos de plantilla individuales:

![Cuadro de diálogo Editar nombre de anuncio con la opción Anular nombres de anuncio habilitada y el nombre completo del anuncio WKND disponible para edición.](images/ad-name-override.png)

Para volver a la nomenclatura basada en plantillas, siga estos pasos:

1. Abra **[!UICONTROL Editar nombre del anuncio]** para el anuncio.
1. Desactivar **[!UICONTROL Anular nombres de anuncios]**.
1. Seleccione **[!UICONTROL Guardar]**.
1. Seleccione **[!UICONTROL Generar nombre de anuncio]** sobre la tabla de activación.

Esta acción también regenera los nombres de otros anuncios de la tabla que tienen una plantilla asignada y no tienen sobrescritura de nombre personalizado.

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

[!DNL GenStudio for Performance Marketing] envía el nombre final de cada anuncio a la plataforma de destino como nombre de anuncio. El nombre enviado incluye cualquier edición de los campos de plantilla o sobrescrituras de nombres personalizados. Los nombres de los anuncios de la plataforma coinciden exactamente con los nombres finales que ha revisado.

Para destinos de visualización como Innovid, los nombres aparecen como nombres creativos.
