---
title: Añadir directrices a Adobe GenStudio for Performance Marketing
description: Aprenda a añadir directrices como parámetros para las peticiones de datos en Adobe GenStudio for Performance Marketing.
feature: Brand Personalization, Product Personalization, Persona Personalization, Variant Generation, Generative AI
role: User
level: Beginner
exl-id: cb893b5d-b535-42f6-8dd8-8bd779d80a4f
source-git-commit: a4df9c81339a8fe5197200d58abc8b48df59da6f
workflow-type: tm+mt
source-wordcount: '2476'
ht-degree: 0%

---

# Adición de directrices

GenStudio for Performance Marketing le permite establecer directrices definidas por el usuario que garantizan que cualquier contenido generado por IA se personalice para alinearse con la identidad de una marca. Esta página ofrece instrucciones para configurar y utilizar cada directriz disponible específica. Para obtener una explicación general, vea la [descripción general de las directrices](/help/user-guide/guidelines/overview.md).

Añadir directrices a GenStudio for Performance Marketing es un paso importante en el proceso de creación. Las directrices informan el proceso de creación de contenido, junto con mensajes definidos por el usuario, [comprobaciones de accesibilidad y contenido](overview.md#compliance) y la tecnología de IA generativa de Adobe para crear recursos impactantes.

Las directrices pueden estar definidas por el usuario o pueden existir como directrices predeterminadas, como [default [!DNL Brand] channel guidelines](/help/user-guide/guidelines/brands.md#default-channel-guidelines).

Al crear variantes a partir de una plantilla con directrices de canal predefinidas (como [!DNL Brands], [!DNL Personas] o [!DNL Products]), estas directrices se aplican a las variantes. Si lo desea, puede cambiarlos.

{{in-academy}}

## Añadir marcas

Para agregar [!DNL Brand], [carga una guía de marca](#upload-a-brand) o [crea manualmente una marca](#manually-add-brand) seleccionando directrices e introduciendo los detalles de tu marca. [Publicar [!DNL Brand]](#publish-brand) en [!DNL Content] para que esté disponible para usarla en futuras generaciones de contenido.

En el área de navegación izquierda, haga clic en **[!DNL Brands]** de la lista _Compartido_.

![Directrices en GenStudio for Performance Marketing](/help/assets/guidelines.png){width="650" zoomable="yes"}

Si carga directrices de marca escritas en un idioma que no sea inglés (o crea manualmente una marca en un idioma que no sea inglés), GenStudio for Performance Marketing muestra esas directrices en ese mismo idioma.

>[!TIP]
>
>Cada marca opera de forma independiente sin relaciones jerárquicas. Para crear submarcas en una marca principal, incluya la información de la marca principal durante el proceso de creación.

### Cargar una marca

Puede cargar sus propios documentos de directrices de marca (hasta tres archivos PDF o DOC) en GenStudio for Performance Marketing para crear automáticamente una marca.

Ver [[!DNL Brands]](/help/user-guide/guidelines/brands.md).

**Para cargar documentos de marca**:

1. En el panel _[!DNL Brands]_, seleccione el botón **[!UICONTROL Agregar marca]**.
1. Elija **[!UICONTROL Cargar PDF]** e introduzca un nombre de marca en la ventana emergente _Elija una forma de agregar su marca_.
1. Seleccione **[!UICONTROL Continuar]**.
1. Examine y adjunte o arrastre sus documentos de directrices de marca a la ventana emergente _[!UICONTROL Agregar su marca]_.

   Puede adjuntar hasta cinco archivos PDF para un máximo de 500 MB.

1. Seleccione **[!UICONTROL Agregar marca]**.

   Con la tecnología de IA generativa de Adobe, GenStudio for Performance Marketing extrae información de los documentos cargados y comienza a crear su marca. La información de la marca, como la voz de la marca, el canal y las directrices de imagen, se rellena a medida que se ensamblan las directrices de los documentos de marca.

Se abre la vista de la nueva marca, que muestra los detalles de las directrices de marca extraídos de los documentos. Una ventana emergente le notifica _&quot;Su marca está lista para revisarse&quot;_ y le recuerda que revise el contenido extraído y realice las modificaciones necesarias.

### Añadir marca manualmente

Puede agregar manualmente los detalles de la marca, en lugar de cargar documentos de marca existentes, para rellenar una nueva [marca](brands.md).

**Para agregar manualmente una marca**:

1. Seleccione el botón **[!UICONTROL Agregar marca]**.
1. Elija **[!UICONTROL Cargar manualmente]** e introduzca un nombre de marca en la ventana emergente _Elija una forma de agregar su marca_.
1. Seleccione **[!UICONTROL Agregar marca]**.

   Se crea y se muestra una nueva marca en blanco.

1. Rellene varios datos, directrices e imágenes de marca para crear su marca en las secciones correspondientes (vistas de pestaña en la parte superior).

   Puede agregar directrices directamente desde la vista de página principal de su nueva marca _o_. Puede agregarlas en las secciones con fichas individuales (que incluyen información sobre herramientas _Ver ejemplos_ para guiarlo) en la parte superior.

   ![Marcas](/help/assets/brands.png){width="600" zoomable="yes"}

   - _Cuándo usar esta marca_: Haz clic en **[!UICONTROL Agregar]** (o haz clic en el campo de texto para cambiar el texto existente) e introduce información general e información de uso sobre la marca. Haga clic en **[!UICONTROL Guardar cambios]**.
   - [_[!DNL Brand] directrices de voz _](brands.md#brand-voice-guidelines): Agregue información aplicable en cada campo de directrices.

     ![Agregar [!DNL Brand] directrices de voz ](/help/assets/brand-voice-add.png){width="500" zoomable="yes"}

   - [_Directrices de imagen_](brands.md#image-guidelines): haga clic en **[!UICONTROL Agregar categoría]** para agregar categorías de guía como &quot;Directrices generales de arte&quot; o &quot;Fotografía de producto&quot;. Rellene las directrices en cada categoría añadida.
   - [_Directrices de canal_](brands.md#channel-guidelines): haga clic en cada canal disponible y agregue las directrices correspondientes.
   - [_Logotipos_](brands.md#logos): haga clic en **[!UICONTROL Agregar logotipo]** para arrastrar y soltar o examinar los logotipos para cargarlos.
   - [_Colores_](brands.md#colors): Haz clic en **[!UICONTROL Agregar color]** para usar un código de color hexadecimal o RGB, o el selector de color, para agregar colores individuales.

     ![Colores de marca](/help/assets/colors.png){width="600" zoomable="yes"}

Para ver su [!DNL Brands] creado, haga clic en la flecha hacia atrás cerca de la parte superior del panel _[!UICONTROL Marcas]_ para volver a la página de inicio de _[!UICONTROL Marcas]_.

No tiene que [publicar](#publish-brand) su [!DNL Brand] para que la información sea accesible. Cualquier información añadida manualmente está disponible inmediatamente después de agregarse. Para que otros miembros de su organización utilicen la información de [!DNL Brand] en GenStudio for Performance Marketing, debe publicarla. Un(a) [!DNL Brand] creado está en forma de borrador hasta su publicación.

### Cambiar miniatura de marca

Después de agregar manualmente un(a) [!DNL Brand], puede cambiar la imagen en miniatura para asegurarse de que se pueda distinguir fácilmente dentro de su lista de [!DNL Brands].

Si se crea un(a) [!DNL Brand] con extracción de documento (en lugar de agregarse manualmente), se implementa automáticamente un logotipo disponible dentro de esos documentos como imagen en miniatura.

**Cambiar manualmente la imagen en miniatura de[!DNL Brand]**:

1. Seleccione **[!UICONTROL Cambiar miniatura]** en el menú de acciones.
1. Cargar una nueva imagen en la ficha _Cargar_.
1. En _[!UICONTROL Cambiar miniatura]_, cambie la imagen cargada.
1. Seleccione **[!UICONTROL Actualizar]** para guardar la imagen como su imagen en miniatura de [!DNL Brand].

Puede seleccionar un logotipo de [!DNL Brand] existente en la vista de la ficha [!UICONTROL Logotipos] para [!DNL Brand]. Haga clic para abrir un logotipo y seleccione **[!UICONTROL Usar como miniatura de marca]** en el menú de acción.

### Publicar marca

Antes de publicar un borrador de [!DNL Brand], haga clic en todas las secciones de directrices para revisar toda la información rellenada. Realice los cambios necesarios en las directrices de marca.

En _[!DNL Brands]_, cualquier borrador o [!DNL Brands] publicado aparecerá como mosaico. En la parte inferior de cada mosaico se muestra una insignia de estado (_ Publicado _o_ Borrador _) y la última vez que se modificó la marca.

>[!TIP]
>
>Si solo desea ver las marcas que ha creado, seleccione **[!UICONTROL Creado por usted]** en el filtro [!DNL Brands] (icono de funnel).

**Para publicar un borrador de marca**:

1. En el área de navegación izquierda, haga clic en **[!UICONTROL [!DNL Brands]]**.
1. Haga clic en un mosaico de miniaturas para abrir un borrador de [!DNL Brand] existente.
1. Haga clic en el botón **[!UICONTROL Publicar]** (solo disponible para borradores).
1. En la ventana emergente _Publicar marca_, verifique quién tiene acceso para ver y usar la [!DNL Brand] publicada.
1. En la ventana emergente _Publicar marca_ que aparece, seleccione **[!UICONTROL Publicar]**.

   La ventana emergente confirma que [!DNL brand] se ha publicado—&quot;{Brand} ya está listo&quot;.

1. Haga clic en **[!UICONTROL Listo]** para salir de la ventana emergente.

[!DNL brand] muestra un punto verde y &quot;Publicado&quot; junto al nombre, y aparece un botón **[!UICONTROL Editar[!DNL brand]]** en lugar del botón **[!UICONTROL Publicar]**.

**Para cancelar la publicación de un(a)[!DNL brand]** publicado(a), haga clic en la marca para abrirlo y luego en **[!UICONTROL Cancelar la publicación]** en el menú de acciones (icono de tres puntos).

La marca publicada ya está disponible para su uso en [_[!DNL Create]_](/help/user-guide/create/overview.md) y [_[!DNL Content]_](/help/user-guide/content/overview.md).

### Administrar marcas

En la página de inicio _[!DNL Brands]_, puede hacer clic en para abrir una marca ya creada con el fin de administrarla o publicarla.

Para **ver la información de marca**, haz clic en **[!UICONTROL [!DNL Brands]]** en el área de navegación izquierda y haz clic para abrir una marca existente.

**Para modificar una marca** en la vista [!DNL Brands]:

1. En **[!DNL Brands]**, haga clic en para abrir una marca definida.
1. Para ver los detalles individuales o modificar las directrices, haga clic en [**[!UICONTROL Directrices de voz de marca]**](brands.md#brand-voice-guidelines), [**[!UICONTROL Directrices de imagen]**](brands.md#image-guidelines), [**[!UICONTROL Directrices de canal]**](brands.md#channel-guidelines), [**[!UICONTROL Logotipos]**](brands.md#logos) o [**[!DNL Colors]**](brands.md#colors) en la parte superior.
1. Para administrar el logotipo de una marca, haz clic en [**[!UICONTROL Logotipos]**](brands.md#logos) en la parte superior y haz clic en el menú de acción (tres puntos).
   1. Seleccione **[!UICONTROL Ver detalles]** para ver información de [!DNL Brand], como _Formato_ y _Tamaño_.
   1. Seleccione **[!UICONTROL Descargar]** para descargar el logotipo.
   1. Seleccione [**[!UICONTROL Usar como miniatura de marca]](#change-brand-thumbnail) para establecer el logotipo como imagen en miniatura.
   1. Seleccione **[!UICONTROL Rename]** para cambiar el nombre del logotipo.
   1. Seleccione **[!UICONTROL Eliminar]** para eliminar el logotipo.
1. Para cambiar el nombre de una marca existente, haga clic en el título e introduzca uno nuevo.
1. Para duplicar una marca existente, selecciona **[!UICONTROL Duplicate]** del menú de acción _[!DNL Brands]_.
   1. Escriba un nombre de marca en la ventana emergente _Marca duplicada_ y haga clic en **[!UICONTROL Marca duplicada]**.

      La ventana emergente confirma que la marca está duplicada: &quot;Nueva marca creada&quot;. La marca duplicada está inicialmente en modo _Sin publicar_.

   1. Personalice la marca duplicada y luego [publíquela](#publish-brand) para que esté disponible para su uso.
1. Para eliminar una marca, selecciona **[!UICONTROL Eliminar]** en el menú de acción [!DNL Brands].

## Agregar [!DNL Personas]

Para agregar una persona, [sube una persona](#upload-a-persona) o [crea manualmente una persona](#manually-add-persona) seleccionando directrices e introduciendo tus detalles de persona.

En el área de navegación izquierda, haga clic en **[!DNL Personas]** de la lista _Compartido_.

![Directrices en GenStudio for Performance Marketing](/help/assets/guidelines.png){width="650" zoomable="yes"}

Puede agregar [!DNL Persona] en GenStudio for Performance Marketing para ayudar a dirigir el contenido que cree a su audiencia ideal.

Ver [[!DNL Personas]](personas.md).

### Cargar una persona

Puede cargar sus propios documentos de personalidad para rellenar nuevos perfiles.

Ver [[!DNL Personas]](/help/user-guide/guidelines/personas.md).

1. En el panel _[!DNL Personas]_, seleccione el botón **[!UICONTROL Agregar persona]**.
1. Elija **[!UICONTROL Cargar archivos]** e introduzca un nombre de persona en la ventana emergente _Elija una forma de agregar su persona_.
1. Seleccione **[!UICONTROL Continuar]**.
1. Examine y adjunte o arrastre sus documentos de directrices de personalidad a la ventana emergente _[!UICONTROL Agregar su personalidad]_.

   Puede adjuntar hasta cinco archivos PDF o DOC por un máximo de 500 MB.

1. Seleccione **[!UICONTROL Agregar personalidades]**.

   Con la tecnología de IA generativa de Adobe, GenStudio for Performance Marketing extrae información de los documentos cargados y comienza a crear su personalidad. A medida que se reúne cada directriz de sus documentos personales, verá detalles como la voz personal, el canal y las directrices de imagen.

   Se abrirá la vista de la nueva persona, en la que se mostrarán los detalles de las directrices de personalidad extraídos de los documentos. Una ventana emergente le notifica _&quot;Su perfil está listo para revisarse&quot;_ y le recuerda que revise el contenido extraído y realice las modificaciones necesarias.

### Añadir persona manualmente

Puede agregar manualmente los detalles de la persona, en lugar de cargar documentos de persona existentes, para rellenar una nueva [persona](personas.md).

**Para agregar manualmente un perfil**:

1. Seleccione el botón **[!UICONTROL Agregar persona]** y elija **[!UICONTROL Agregar manualmente]**.
1. Haga clic en **[!UICONTROL Continuar]**.

   Puede rellenar varias directrices e imágenes opcionales para crear su personalidad.

1. Haga clic en **[!UICONTROL Nuevo nombre de persona]** e introduzca un nombre para [!DNL Persona].
1. Agregue información sobre su [!DNL Persona] en la sección _Descripción_.

   ![Agregar un(a) [!DNL Persona]](/help/assets/personas-add.png){width="650" zoomable="yes"}

1. Haga clic en _Descripción_ e introduzca una descripción de este(a) [!DNL Persona].
1. Haz clic en _Preferencias de mensajería_ e introduce los detalles de mensajería para [!DNL Persona].
1. Para editar la miniatura, pasa el ratón sobre ella y, en el menú de acciones, selecciona **[!UICONTROL Editar miniatura]**.
   1. Elija una imagen de la galería en la ficha _Galería_ _o_ cargue una nueva imagen en la ficha _Cargar_.

      También puede eliminar o recortar una imagen en miniatura existente en la ficha _Cargar_.

   1. Haga clic en **[!UICONTROL Usar imagen]**.
1. Para editar la imagen de portada, pasa el ratón sobre la portada y en el menú de acciones selecciona **[!UICONTROL Editar portada]**.
   1. Elija una imagen de la galería en la ficha _Galería_ _o_ cargue una nueva imagen en la ficha _Cargar_.
   1. Haga clic en **[!UICONTROL Usar imagen]**.
   1. Para cambiar la posición de la imagen de portada, haga clic en **[!UICONTROL Cambiar posición]** en el menú de acción, arrastre la imagen a la posición deseada y haga clic en **[!UICONTROL Guardar]**.

   Para ver su [!DNL Personas] creado, haga clic en la flecha hacia atrás cerca de la parte superior de la vista _Persona_ para volver a la página de inicio de _[!DNL Personas]_.

### Administrar [!DNL Personas]

En la página de inicio de _[!DNL Personas]_, puedes **abrir un elemento[!DNL Persona]**ya creado para editarlo o revisarlo, o **eliminar un elemento personal**de la lista:

- Seleccione **[!UICONTROL Abrir]** en el menú de acciones de [!DNL Personas] para revisar un perfil existente.
- Seleccione **[!UICONTROL Eliminar]** del menú de acción [!DNL Personas] para **eliminar** una persona.
- Seleccione **[!UICONTROL Cambiar nombre]** del menú de acción [!DNL Personas] para **Cambiar nombre** de persona.

## Agregar [!DNL Products]

Para agregar un producto:

1. En el área de navegación izquierda, haga clic en **[!DNL Products]** de la lista _Compartido_.
   ![Directrices en GenStudio for Performance Marketing](/help/assets/guidelines.png){width="650" zoomable="yes"}
1. En el panel _[!DNL Products]_, seleccione **Agregar producto**.
1. Elija [cargar un producto](#upload-a-product) o [crear manualmente un producto](#manually-add-product) seleccionando directrices e introduciendo los detalles del producto.

![Agregar un(a) [!DNL Product]](/help/assets/products-add.png){width="650" zoomable="yes"}

Puede incluir a [!DNL Product] en GenStudio for Performance Marketing para adaptar mejor el contenido que crea para un producto específico.

Ver [[!DNL Products]](products.md).

### Cargar un producto

Puede cargar sus propios documentos de producto para rellenar nuevos productos.

Ver [[!DNL Products]](/help/user-guide/guidelines/products.md).

1. Seleccione el botón **[!UICONTROL Agregar producto]**.
1. Elija **[!UICONTROL Cargar archivos]** e introduzca un nombre de producto en la ventana emergente _Elija una forma de agregar su producto_.
1. Seleccione **[!UICONTROL Continuar]**.
1. Examine y adjunte o arrastre sus documentos de directrices de productos a la ventana emergente _[!UICONTROL Agregar su producto]_.

   Puede adjuntar hasta cinco archivos PDF o DOC por un máximo de 500 MB.

1. Seleccione **[!UICONTROL Agregar productos]**.

   Con la tecnología de IA generativa de Adobe, GenStudio for Performance Marketing analiza los documentos cargados para crear el perfil del producto. A medida que se procesa cada directriz de los documentos del producto, verá información como las descripciones de los productos, las propuestas de valores y las preferencias de mensajería.

   Se abre la vista del nuevo producto, que muestra los detalles de las directrices del producto extraídas de los documentos. Una ventana emergente le notifica _&quot;Su producto está listo para revisarse&quot;_ y le recuerda que revise el contenido extraído y realice las modificaciones necesarias.

### Añadir manualmente un producto

Puede agregar manualmente los detalles del producto, en lugar de cargar documentos de producto existentes, para rellenar [productos](products.md) nuevos.

**Para agregar manualmente un producto**:

1. Seleccione el botón **[!UICONTROL Agregar producto]** y elija **[!UICONTROL Agregar manualmente]**.
1. Haga clic en **[!UICONTROL Continuar]**.

   Puede rellenar varios datos opcionales para crear el producto.

1. Haga clic en **[!UICONTROL Nuevo nombre de producto]** e introduzca un nombre para [!DNL product].
1. Agregue información sobre su [!DNL product] en la sección _Descripción_.
1. Haga clic en _Descripción_ e introduzca una descripción de este(a) [!DNL Product].
1. Haga clic en _Propuesta de valor_ e introduzca los detalles de la propuesta de valor para colocar correctamente su [!DNL Product].
1. Haz clic en _Preferencias de mensajería_ e introduce los detalles de mensajería para [!DNL product].
1. Para editar la miniatura, pasa el ratón sobre ella y, en el menú de acciones, selecciona **[!UICONTROL Editar miniatura]**.
   1. Elija una imagen de la galería en la ficha _Galería_ _o_ cargue una nueva imagen en la ficha _Cargar_.

      También puede eliminar o recortar una imagen en miniatura existente en la ficha _Cargar_.

   1. Haga clic en **[!UICONTROL Usar imagen]**.
   1. Para editar la imagen de portada, pasa el ratón sobre la portada y en el menú de acciones selecciona **[!UICONTROL Editar portada]**.
   1. Elija una imagen de la galería en la ficha _Galería_ _o_ cargue una nueva imagen en la ficha _Cargar_.
   1. Haga clic en **[!UICONTROL Usar imagen]**.
   1. Para cambiar la posición de la imagen de portada, haga clic en **[!UICONTROL Cambiar posición]** en el menú de acción, arrastre la imagen a la posición deseada y haga clic en **[!UICONTROL Guardar]**.

   Para ver su [!DNL Products] creado, haga clic en la flecha hacia atrás cerca de la parte superior de la vista _Producto_ para volver a la página de inicio de _[!DNL Products]_.

### Administrar [!DNL Products]

En el inicio de _[!DNL Products]_, puede **abrir un elemento[!DNL Product]**ya creado para editarlo o revisarlo, o **eliminar un producto**de la lista:

- Seleccione **[!UICONTROL Abrir]** del menú de acciones [!DNL Products] para revisar un producto existente.
- Seleccione **[!UICONTROL Eliminar]** del menú de acción [!DNL Products] para **eliminar** un producto.
- Seleccione **[!UICONTROL Rename]** del menú de acción [!DNL Products] para **Rename** un producto.

## Agregar [!DNL Audiences]

>[!NOTE]
>
>La característica [!DNL Audiences] requiere la incorporación del equipo de Adobe para que aparezca en GenStudio. Si _[!DNL Audiences]_no aparece en los parámetros de la plantilla, comuníquese con el representante de Adobe.

[!DNL Audiences] proporciona segmentos de clientes segmentados desde Adobe Real-Time Customer Data Platform (RTCDP), lo que aporta datos de segmentación precisos al flujo de trabajo de generación de contenido. GenStudio for Performance Marketing aprovecha las definiciones de audiencia para ayudarle a crear contenido de marketing personalizado y adaptado a segmentos de clientes específicos.

[!DNL Audiences] aparece como una lista desplegable en el panel de parámetros, en [el flujo de trabajo _[!DNL Create]_](../create/overview.md#templates)._[!DNL Audiences]_ puede agregar especificidad a _[!DNL Personas]_cuando se utilizan ambas directrices, pero también se puede utilizar de forma independiente de forma eficaz.

Durante la incorporación, las definiciones de audiencia se importan y transforman en un formato compatible con GenStudio. Este proceso suele tardar unos días en completarse. Póngase en contacto con el equipo de Adobe para iniciarlo.

**Requisitos previos**:

- Acceso de la organización a Adobe Real-Time Customer Data Platform
- Audiencias existentes ya configuradas en los entornos limitados de RTCDP
- La integración de _[!DNL Audience]_requiere un proceso de incorporación manual por parte del equipo de Adobe

**Para seleccionar una audiencia**:

1. En [el flujo de trabajo _[!DNL Create]_](../create/overview.md#templates), seleccione una plantilla y haga clic en el botón **[!UICONTROL Usar]**para abrir el borrador.
1. En la lista de parámetros, haga clic en el menú desplegable _[!UICONTROL Audiencia]_ para ver todas las audiencias disponibles.
   ![Menú desplegable Audiencia en el panel Parámetros personales](./audience-dropdown.png){width=450}
1. Seleccione una audiencia para asignarla de la lista. El sistema sugiere audiencias recomendadas que se alinean con los [!DNL Persona] seleccionados, si se ha seleccionado un [!DNL Persona].
1. Haga clic en **[!UICONTROL Ver detalles de la audiencia]** para ver la descripción ampliada y las preferencias de mensajería generadas para la audiencia seleccionada. Los detalles de la audiencia informan la generación de contenido, lo que garantiza que el creativo se ajuste a las características y preferencias específicas del segmento de destino.
   ![Panel de detalles de audiencia](./audience-details.png){width=450}
