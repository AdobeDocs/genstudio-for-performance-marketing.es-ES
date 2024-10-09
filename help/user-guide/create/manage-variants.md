---
title: Administrar variantes
description: Personalice y mejore las variantes y los recursos generados para adaptarlos a sus necesidades de marketing digital.
feature: Content, Assets, Experiences
source-git-commit: 157aee296304c9aa1b8b86dc8905fe103fe4f83c
workflow-type: tm+mt
source-wordcount: '995'
ht-degree: 0%

---


# Administrar variantes

Adobe GenStudio for Performance Marketing [!DNL Create] le permite personalizar y mejorar variantes generadas ([correos electrónicos](/help/user-guide/create/email-experiences.md), [anuncios Meta](/help/user-guide/create/meta-experiences.md) y más) para usarlas en iniciativas de marketing digital.

Al [crear experiencias](/help/user-guide/create/overview.md), puede modificar el contenido y los recursos de variantes generadas de forma individual o en lote. La capacidad de administrar variantes en el micro nivel individual le permite administrar explícitamente cada parte del contenido generado.

## Cambiar nombre de borrador

Los borradores de variante generados tienen un nombre predeterminado que se muestra en la parte superior del lienzo. Los nombres de borrador predeterminados utilizan la siguiente convención que incluye el tipo de canal, la fecha y la hora de generación.

*Ejemplo*: &quot;Meta: Borrador sin título - 09.5.24, 9:56 AM&quot;

**Para cambiar el nombre predeterminado**:

1. Después de generar un conjunto de variantes, haga clic en el nombre predeterminado _Borrador sin título_ en la parte superior del lienzo.
1. Seleccione texto e introduzca un nombre nuevo.
1. Haga clic fuera del campo de texto para guardarlo.

## Editar texto manualmente

Puede editar los campos de texto en las variantes generadas. Refine el texto para su audiencia experimentando con diferentes frases y expresiones. Por ejemplo, puede revisar manualmente el texto en variantes para previsualizar el aspecto de un titular con una imagen elegida.

**Para editar texto manualmente en variantes generadas**:

1. Después de generar un conjunto de variantes, haga doble clic en el texto editable de una variante.
1. Introduzca el nuevo texto.
1. Haga clic fuera del campo de texto para guardarlo.

<!-- ## Re-generate sections

GenStudio for Performance Marketing has the built-in functionality to regenerate single sections of generated variants using _[!UICONTROL Suggested edits]_ and fresh prompts.

For example, you can re-generate the headline section of one Meta ad variant to see how it looks with a specific background asset using the _[!UICONTROL Suggested edits]_ options—_[!UICONTROL Rephrase]_, _[!UICONTROL Shorten]_, or _[!UICONTROL Lengthen]_—and entering a new prompt.

**To re-generate individual variant sections**:

1. After generating a set of variants, single-click editable text in a variant.
1. (_Optional_) Enter a new prompt to change the focus of the regenerated content.
1. Select a _[!UICONTROL Suggested edits]_ option—_[!UICONTROL Rephrase]_, _[!UICONTROL Shorten]_, or _[!UICONTROL Lengthen]_.
1. Click **[!UICONTROL Generate]**.
1. If you want to regenerate results, click the regenerate icon adjacent to _Results_.
1. From the _Results_ that appear, select the desired option and click **[!UICONTROL Replace]**.

   The variant is updated with the revised text. -->

## Recortar recursos

Puede recortar y cambiar manualmente la posición de los recursos de imagen en variantes generadas individualmente.

**Para recortar y cambiar la posición de imágenes en variantes**:

1. Después de generar un conjunto de variantes, pase el ratón sobre una imagen dentro de una variante.
1. Haga clic en el icono de recorte que aparece en la esquina izquierda de la imagen.
1. Ajuste el cuadro delimitador de la imagen y arrastre la imagen a la posición deseada.
1. Haga clic en **[!UICONTROL Aplicar]** para aplicar el recorte a una sola imagen o en **[!UICONTROL Aplicar a todas las imágenes]** para aplicar a todas las imágenes de las variantes.

   La imagen recortada se guarda y es visible para las variantes.

## Cambiar proporción de aspecto

Puede cambiar rápidamente la proporción de aspecto de los anuncios Meta para adaptarse al tamaño de anuncio deseado.

Las relaciones de tamaño y aspecto disponibles son:

* Cuadrado 1:1 (Meta)
* 4:5 vertical (Meta)
* 9:16 vertical (Meta)
* 250 x 980 (anuncio en pantalla)

>[!NOTE]
>
>Pueden estar disponibles otros tamaños y relaciones de aspecto en función de las plantillas disponibles.

**Para cambiar la proporción de aspecto de los Meta ads generados**:

1. Después de generar un conjunto de variantes, seleccione el icono de cambio de tamaño de la relación de aspecto (la flecha que señala a la esquina del cuadro) en el lado izquierdo del lienzo.

   La proporción de aspecto que se usa actualmente para tus anuncios se muestra en la parte superior de la ventana _[!UICONTROL Cambiar tamaño]_.

   El número de variaciones afectadas por esta revisión se indica en la esquina superior derecha de la ventana. _Ejemplo_: &quot;4 de 4 variaciones&quot;

1. Seleccione una relación de aspecto disponible.

   Solo se pueden elegir los tamaños de relación de aspecto que no se representan actualmente en el lienzo.

1. Haga clic en **[!UICONTROL Duplicar y cambiar tamaño]**.

   [!DNL Create] crea una copia de cada variante en función de la nueva proporción de aspecto seleccionada. Todas las variantes, incluidas las de la relación de aspecto inicial, están presentes en el lienzo.

   Por ejemplo, si genera cuatro variantes en una relación de aspecto de 1:1 inicialmente y luego cambia la relación de aspecto a 4:5, ahora habrá _ocho_ variantes totales disponibles en el lienzo.

## Intercambiar imagen

Puede añadir o intercambiar imágenes en variantes generadas directamente desde el lienzo.

**Para agregar o intercambiar imágenes en una variante**:

1. Después de generar un conjunto de variantes, haga clic en un recurso de imagen.

   Si la variante no tiene actualmente un recurso de imagen colocado, haga clic en el área del recurso de imagen.

1. Para seleccionar un recurso de imagen ya publicado en [!DNL Content]:
   1. Haga clic en **[!UICONTROL Seleccionar del contenido]**. Utilice los filtros para restringir aún más los resultados de búsqueda.
   1. Haga clic en **[!UICONTROL Usar]**
1. Para cargar un recurso de imagen:
   1. Haga clic en **[!UICONTROL Cargar nueva imagen]** para examinar los archivos y elegir los recursos que desea utilizar. Además de explorar el dispositivo, puede importar desde Microsoft OneDrive o Dropbox.
   1. Haga clic en **[!UICONTROL Agregar Assets]**.

   Las imágenes se añaden o se intercambian en la variante aplicable.

## Vista previa del dispositivo

Al revisar y preparar las experiencias de correo electrónico, puede alternar entre vistas previas para escritorio y vistas móviles para garantizar la coherencia y el atractivo visual de las variantes de borrador.

**Para obtener una vista previa de las variantes para equipos de escritorio y dispositivos móviles**, alterne la opción de vista previa del dispositivo (entre **escritorio** y **móvil**) en la barra de menú derecha (iconos del equipo y del teléfono) para obtener una vista previa del aspecto de las variantes.

## Eliminar variante

Puede eliminar cualquier variante generada que no vaya a guardar ni reutilizar.

Elimine variantes innecesarias para que el lienzo de trabajo muestre solo las variantes que está refinando o utilizando de forma activa.

**Para eliminar una variante generada**:

1. Después de generar un conjunto de variantes, haga clic en el icono de opciones (tres puntos) sobre una variante.

   La variante se realza y aparece un menú de accesos directos.

1. Seleccione **[!UICONTROL Eliminar]** de las opciones disponibles.

   Se elimina la variante.

## Validación de marca por variante

Use la _[!UICONTROL comprobación de directrices de marca]_ y el _[!UICONTROL panel de validación de marca]_ para mantener una identidad de marca y una alineación coherentes de las variantes.

Consulte [Validación de marca](/help/user-guide/guidelines/brand-validation.md#improve-brand-alignment).

## Comentarios de generación

Se pueden enviar comentarios sobre la calidad de los recursos alineados con la marca generados para mejorar el proceso de generación de contenido. La indicación de si los resultados son de alta o baja calidad ayuda a mejorar la calidad general del contenido y la seguridad del usuario en GenStudio for Performance Marketing.

Los comentarios de generación se aplican a una variante individual, no al conjunto recopilado de variantes.

**Para enviar comentarios de generación**:

1. Después de generar un conjunto de variantes, haga clic en el icono de opciones (tres puntos) sobre una variante.

   La variante se realza y aparece un menú de accesos directos.

1. Seleccione **[!UICONTROL Buen resultado]** o **[!UICONTROL Mal resultado]**.

   Aparecerá una ventana emergente de comentarios para recopilar más información. El contenido generado y la información del mensaje se incluyen en sus comentarios.

1. Añada la siguiente información en la ventana emergente de comentarios:
   1. Seleccione la opción _[!UICONTROL Incluir también el contenido de referencia y los datos de capa]_ para incluir esa información de referencia adicional en los comentarios recopilados.
   1. De _[!UICONTROL ¿Qué funcionó bien?]_ o _[!UICONTROL ¿Qué ha fallado?]_, seleccione las opciones que describen qué hace que la generación de contenido sea de alta o baja calidad.
   1. Agregue cualquier otra información útil o relacionada en el campo _[!UICONTROL Notas]_.
1. Haga clic en **[!UICONTROL Enviar]**.

   Aparecerá un banner para confirmar que ha enviado comentarios.
