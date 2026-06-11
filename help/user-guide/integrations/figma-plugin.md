---
title: Complemento Figma para Adobe GenStudio for Performance Marketing
description: Aprenda a configurar y utilizar el complemento Figma para GenStudio for Performance Marketing.
feature: Generative AI
role: User
exl-id: 232fbbc6-c523-4525-8d26-a8ac8d62c035
TQID: https://experienceleague.adobe.com/JKHpT5m-4KZvq-iWF2u11hRaFFRhKMo-ofbWk-xvRMI
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: e0aa398c-6185-4e77-8cf7-2561c578c181
subfeature_v2:
  - id: f8fb16a4-19e5-44e1-8db9-d45f8e266e2c
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 2c5e5166bfe9d4b1c6cb56495613ff5cf20fab34
workflow-type: tm+mt
source-wordcount: 1793
ht-degree: 76%

---

# Complemento Figma para GenStudio for Performance Marketing

El complemento GenStudio for Performance Marketing Figma añade un nuevo panel a la aplicación Figma que le permite generar contenido propio de la marca.
[Busque e instale el complemento desde el mercado de la comunidad Figma](https://www.figma.com/community/plugin/1604251370122180013/firefly-enterprise-and-genstudio).

Esta página describe cómo configurar y utilizar el complemento.

Las funciones de este complemento incluyen:

* Asigne elementos de texto de Figma a campos de GenStudio for Performance Marketing como `headline`, `body`, `on_image_text` y más.
* Generar un nuevo anuncio en la marca Meta, LinkedIn o Display [!DNL Experiences] basado en una marca, personalidad, producto y mensaje de texto.
* Cree [!DNL Experiences] directamente en el documento de Figma reemplazando el texto de los elementos de Figma asignados con los valores generados por GenStudio for Performance Marketing.
* Reformule, acorte, alargue o traduzca contenido existente en función de un mensaje.
* Traducir [!DNL Experiences] generado a varios idiomas.
* Exportar [!DNL Experiences] generado a un origen local como imágenes aplanadas.
* Exportar [!DNL Experiences] generado a GenStudio for Performance Marketing.
* Utilice opciones de plugin que se adapten a los elementos seleccionados en el lienzo Figma.

>[!VIDEO](https://video.tv.adobe.com/v/3478812?captions=spa&learn=on)

## Creación de una plantilla

El complemento requiere los dos primeros niveles del documento de Figma para seguir esta convención:

* **Sección**: representa el proyecto principal, que puede contener varias plantillas.
* **Marco**: representa una plantilla dentro de un proyecto. La plantilla se puede rellenar con texto, imágenes, componentes y otros elementos.

### Meta templates

Se admiten estos tamaños de plantilla:

Para publicaciones de Instagram o Facebook:

* Anchura: 1080 px (fija)
* Altura: 1080 px o 1350 px

Para historias de Instagram o Facebook:

* Anchura: 1080 px (fija)
* Altura: 1920 px

El complemento decide el cromo de la experiencia generada en función de la altura de la plantilla.

### Mostrar plantillas

No hay requisitos de tamaño fijo. Las plantillas de visualización admiten cualquier tamaño.

### Plantillas de LinkedIn

* Anchura: 1200 px (fija)
* Altura: 1200 px, 628 px, 2292 px, 1800 px o 1500 px

### Asignación de funciones de campo

El complemento debe comprender los diferentes elementos de la plantilla, como el titular, el texto independiente o la imagen.

**Los roles de campo de Meta incluyen**:

* Imagen
* Texto de imagen
* CTA
* Texto del cuerpo
* Titular
* URL del sitio web
* Mostrar vínculo
* Campos manuales

Consulte cómo se asignan algunas de estas funciones de campo a continuación.

| ![Publicación de Facebook con los roles indicados](./facebook-post.png){width="60%" align="center" zoomable="yes"}<br> | ![Se ha indicado una historia de Facebook con roles de campo](./facebook-story.png){width="70%" align="center" zoomable="yes"}<br> |
|:---:|:---:|
| ![Se ha indicado una publicación de Instagram con funciones de campo](./instagram-post.png){width="60%" align="center" zoomable="yes"}<br> | ![Se ha indicado una historia de Instagram con los roles](./instagram-story.png){width="70%" align="center" zoomable="yes"}<br> |

**Los roles de campo de LinkedIn incluyen**:

* Imagen
* Texto introductorio
* Texto de imagen
* Titular
* CTA
* URL del sitio web
* Campos manuales

Consulte cómo se asignan algunas de estas funciones de campo a continuación.

![Publicación de LinkedIn con los roles de campo indicados](./linkedin-ad.png){width="30%" align="center" zoomable="yes"}

El complemento recuerda estas asignaciones para utilizar con el contenido generado. Una función de campo se puede asignar a varios elementos de plantilla. Los campos manuales son para elementos que desea conservar la comestibilidad del texto, pero que no se marcarán para la generación.

>[!IMPORTANT]
>
> **Debe asignar una imagen** al asignar el rol de campo `image` al menos a un elemento de imagen de la plantilla.

Para asignar roles de elemento:

1. Seleccione un elemento en la plantilla (texto, imagen, etc.).
1. Utilice el menú desplegable para asignar una función.

![Asignación de funciones de campo](./field-role-mapping.png){width="60%" zoomable="yes"}

{{$include /help/_includes/field-mapping-exceptions.md}}

## Generar contenido nuevo

Utilice GenStudio for Performance Marketing AI para generar o realizar variaciones de elementos en plantillas Figma.

1. Si utiliza GenStudio Plugin Playground o ya ha preparado plantillas, seleccione el nodo de la sección que contiene sus plantillas de publicidad. Puede hacerlo desde el panel **Capas** o haciendo clic directamente en la sección del lienzo.
   ![Selección o variaciones de sección](./plugin-playground.png){width="50%" zoomable="yes"}
1. En la ventana del complemento, introduzca un nombre de proyecto para las variaciones, elija una plataforma para el contenido y rellene el resto de la información necesaria. A continuación, haga clic en el botón **[!UICONTROL Finalizar configuración]**.
   ![Ventana del proyecto de instalación](./setup-project.png){width="30%" zoomable="yes"}
1. Seleccione [!DNL Brand], [!DNL Persona] y [!DNL Product] para usar en la generación de contenido.
1. Seleccione el número de variaciones que desea producir (hasta ocho).
1. Use el botón en **[!UICONTROL Seleccionar contenido]** para examinar y elegir imágenes de sus recursos. Los 40 recursos añadidos más recientemente aparecen primero y puede buscar otros recursos. Las imágenes seleccionadas cambian de tamaño automáticamente para adaptarse a las plantillas.
1. Introduzca un mensaje de texto. Cada campo de la lista **[!UICONTROL Campos]** tiene la opción **[!UICONTROL Acción]** establecida en **[!UICONTROL Generar]** para el contenido nuevo.
1. Asigne todas las funciones de campo. Consulte [Asignación de funciones de campo](#field-role-mapping).
1. Haga clic en el botón **[!UICONTROL Generar]**.

## Traducir o generar variaciones de copia de anuncio a partir de contenido existente

Utilice GenStudio for Performance Marketing AI para generar variaciones de copia de anuncios o traducir plantillas Figma.

1. Seleccione el nodo de sección que contiene las plantillas de publicidad. Puede hacerlo desde el panel **Capas** o haciendo clic directamente en la sección del lienzo.
   ![Selección o variaciones de sección](./plugin-playground.png){width="50%" zoomable="yes"}
1. En la ventana del complemento, introduzca un nombre de proyecto para las variaciones y elija una plataforma para el contenido.
1. En **[!UICONTROL ¿Cuál es el objetivo?]**, seleccione **[!UICONTROL Generar variaciones]** o **[!UICONTROL Traducir]** y luego haga clic en el botón **[!UICONTROL Finalizar configuración]**.
   ![Ventana del proyecto de instalación](./setup-project.png){width="30%" zoomable="yes"}
1. Seleccione [!DNL Brand], [!DNL Persona] y [!DNL Product] para usar en la generación de contenido.
1. Seleccione el número de variaciones que desea producir.
1. Use el botón en **[!UICONTROL Seleccionar contenido]** para examinar y elegir imágenes de sus recursos. Los 40 recursos añadidos más recientemente aparecen primero y puede buscar otros recursos. Las imágenes seleccionadas cambian de tamaño automáticamente para adaptarse a las plantillas.
1. Introduzca un mensaje de texto. Cada campo de la lista **[!UICONTROL Campos]** tiene la opción **[!UICONTROL Acción]** establecida en **[!UICONTROL Generar]** para el contenido nuevo.
1. Asigne todas las funciones de campo. Consulte [Asignación de funciones de campo](#field-role-mapping).
1. Seleccione cada tipo de campo para generar variaciones o traducir en el panel de la izquierda del complemento y pegue el contenido inicial en cada cuadro de **[!UICONTROL Contenido inicial]**.
   ![Texto de muestra en el cuadro Contenido inicial](./initial-content-box.png){width="60%" zoomable="yes"}
1. Haga clic en el botón **[!UICONTROL Generar]**.

## Traducir contenido después de la generación

1. Seleccione la generación que desee traducir.
   ![Seleccionar generación](./select-generation.png){width="20%" zoomable="yes"}
1. Elija **[!UICONTROL Traducción]** y luego haga clic en **[!UICONTROL Traducir]**.
1. Seleccione el o los idiomas de destino.
1. Haga clic en **[!UICONTROL Seleccionar]**.

Los resultados de la traducción incluyen:

* Aparece una nueva página con contenido traducido.
* Cada traducción muestra el idioma o la configuración regional de destino.
* El contenido original permanece sin cambios en la página original.

![Resultados de la traducción](./translation-results.png){width="60%" zoomable="yes"}

## Otras acciones en los campos de contenido después de la generación

Cuando edita contenido existente en un campo, aparecen opciones útiles en el panel del complemento.

![Opciones de acciones de complemento](./figma-other-actions.png){width="30%" zoomable="yes"}

Las opciones que se incluyen son:

* Cambie **[!UICONTROL Value]** para modificar el texto directamente. Cambiar este contenido se aplica automáticamente a todas las variaciones seleccionadas.
* La IA puede realizar muchas opciones de **[!UICONTROL Action]**, entre ellas:

| Acción | Descripción |
| --- | --- |
| **[!UICONTROL Generar]** | Generar una nueva variación del texto. |
| **[!UICONTROL Reformular]** | Generar una nueva variación del texto. |
| **[!UICONTROL Acortar]** | Genere una variación más corta del texto. |
| **[!UICONTROL Alargar]** | Generar una variación más larga del texto. |

Después de seleccionar una opción **[!UICONTROL Action]**, vuelva a generar el contenido con el botón **[!UICONTROL Regenerar]**.

## Exportar experiencias

Las variaciones se pueden exportar desde Figma como GenStudio for Performance Marketing [!DNL Experiences].

1. Seleccione el contenido que desea exportar en el lienzo Figma mediante uno de los procedimientos siguientes:
   * Seleccione la sección de generación en el lienzo y, a continuación, haga clic en **[!UICONTROL Marcar todo para exportar]** en el panel del complemento.
     ![Selección de sección de generación](./select-generation-section.png){width="20%" zoomable="yes"}
   * Seleccione una generación individual en el lienzo y, a continuación, haga clic en **[!UICONTROL Marcar para exportación]** en el panel del complemento.
     ![Selección de generación individual](./select-generation.png){width="20%" zoomable="yes"}
1. Seleccione el elemento Exportar del menú de la barra lateral.
   ![Botón Marcar para exportar mostrado para un anuncio de Meta](./mark-for-export.png){width="60%" zoomable="yes"}
1. Seleccione un destino.
1. Haga clic en **[!UICONTROL Exportar]** para exportar el contenido.

Se crea un archivo ZIP en el panel del complemento o aparece un vínculo a **[!UICONTROL Abrir en GenStudio]**. Use el vínculo ZIP para elegir dónde guardar el archivo o seleccione **[!UICONTROL Abrir en GenStudio]**.

## Convertir fotogramas de Figma a Photoshop

>[!NOTE]
>
> Para realizar esta tarea, necesita el complemento Figma y [GenStudio Photoshop](photoshop-plugin.md).

Puede usar el complemento Figma para convertir un marco Figma, varios marcos o un documento completo al formato Photoshop y exportarlo para utilizarlo con [GenStudio Photoshop](photoshop-plugin.md). Actualmente, solo se admiten propiedades principales como visibilidad, tamaño de fuente y atributos de capa básicos durante la conversión. Todavía no se admiten funciones como tachado, superíndice, subíndice, opacidad como porcentajes, degradados y propiedades avanzadas similares.

<!-- GS-34076: Demo video placement is hardcoded in the tool UI; keep this video above "The plugin supports the following Figma layer types for conversion." -->
>[!VIDEO](https://video.tv.adobe.com/v/3492271?learn=on)

El complemento admite los siguientes tipos de capas Figma para la conversión:

* **Cuadro**
* **Grupo**
* **Instancia**
* **Texto**
* **Vector**
* **Imagen**

Cuando se convierte a PSD, las capas admitidas se asignan a Photoshop de la siguiente manera:

| Tipo de capa Figma | Convierte a Photoshop | Notas |
| --- | --- | --- |
| **Cuadro** | Grupo de capas | <ul><li>Los fotogramas de Figma se convierten en grupos de capas de Photoshop.</li><li>Los fotogramas anidados se convierten en grupos anidados.</li><li>Las dimensiones de marco se convierten en la mesa de trabajo o los límites de grupo de PSD (según la selección).</li></ul> |
| **Grupo** | Grupo de capas | <ul><li>Los grupos Figma se convierten directamente en grupos de capas de Photoshop.</li><li>Se conservan la jerarquía de capas y el orden de apilamiento.</li></ul> |
| **Instancia** | Grupo de capas | <ul><li>Los componentes y las instancias se acoplan en grupos de capas estándar de Photoshop. Los metadatos de componente y la lógica de variante no se conservan.</li><li>Todas las capas secundarias permanecen dentro del grupo.</li></ul> |
| **Texto** | Capa de texto | <ul><li>Las capas de texto Figma se convierten en capas de texto Photoshop editables.</li><li>Se conservan la jerarquía y la posición del texto.</li></ul> |
| **Vector** | Capa de forma | <ul><li>Las capas vectoriales de Figma se convierten en capas de forma de Photoshop.</li><li>Las rutas se conservan cuando es posible.</li><li>Los vectores complejos pueden rasterizarse si se aplican efectos no compatibles.</li></ul> |
| **Imagen** | Capa de trama | <ul><li>Las capas de imagen Figma se convierten en capas rasterizadas de Photoshop.</li><li>Se conservan la escala y la posición de las imágenes.</li></ul> |

### Cómo convertir fotogramas

Para convertir fotogramas:

1. Abra el complemento de Firefly Enterprise y GenStudio en Figma y haga clic en la ficha **[!UICONTROL Exportar]** en la interfaz de usuario del complemento.
1. En el lienzo, seleccione el marco o marcos que desea exportar. Puede elegir uno o varios marcos.

   >[!NOTE]
   >
   > Los fotogramas no pueden estar dentro de una sección durante la conversión. Seleccione tramas que no estén anidadas dentro de un nodo de sección.

1. Para migrar los fotogramas seleccionados, realice una de las siguientes acciones:

   * Haga clic en **[!UICONTROL Exportar]** para exportar el archivo convertido a una ubicación elegida o
   * Haga clic en **[!UICONTROL Transferir a Photoshop]** para almacenar en caché el archivo convertido para su uso inmediato en GenStudio Photoshop.
     ![Botón Transferir a GenStudio Photoshop](./transfer-to-ps-button.png){width="40%"}
1. A continuación, comparta el vínculo de archivo Figma. El complemento necesita una URL de archivo Figma para completar la conversión. Añada la dirección URL del documento.

   1. En Figma, haz clic en **[!UICONTROL Compartir]** en la esquina superior derecha del lienzo.
   1. En **[!UICONTROL Compartir este archivo]**, haga clic en **[!UICONTROL Copiar vínculo]**.
   1. Pegue el vínculo copiado en el campo **[!UICONTROL Vínculo de archivo Figma]** del cuadro de diálogo del complemento [!DNL GenStudio for Performance Marketing]. Esto debe hacerse para cada archivo:
      ![Cuadro de diálogo obligatorio con clave de archivo](./file-key-required.png){width="35%"}
   1. Haga clic en **[!UICONTROL Enviar]**.
1. Aparecerá una ventana emergente pidiendo acceso para leer el contenido y los metadatos del archivo. Esto solo debe hacerse una vez para todos los archivos. Haga clic en **[!UICONTROL Permitir acceso]**. El complemento leerá los marcos seleccionados en Figma y los convertirá en un documento JSON, un formato intermedio para los datos del archivo.
   ![Permitir acceso para leer el contenido y los metadatos del archivo](./figma-access-request.png){width="35%"}
1. En Photoshop, abra [!DNL GenStudio Photoshop] y haga clic en la ficha **[!UICONTROL Importar]**.
1. Para seleccionar los archivos convertidos, realice uno de los siguientes pasos:

   * Haga clic en **[!UICONTROL Desde el complemento]** para elegir un archivo convertido con **[!UICONTROL Transferir a GenStudio Photoshop]** de la lista de archivos en caché, o
   * Haga clic en **[!UICONTROL Cargar JSON]** para buscar y seleccionar el archivo JSON que desea cargar.
     ![Botón Cargar JSON](./upload-json.png){width="40%"}
1. GenStudio Photoshop convierte la información del documento JSON en un documento de Photoshop abierto.
1. Haga clic en **[!UICONTROL Listo]**. El nuevo archivo se abre en Photoshop y está listo para usarse. O haga clic en **[!UICONTROL Guardar como...]** para elegir una ubicación donde guardar el archivo.
   ![Cuadro de diálogo de botón Listo](./import-done-button.png){width="40%"}

## Historial de generación

El complemento mantiene un historial de cambios para cada campo. En la página de plantilla, elija **[!UICONTROL Historial de generación]** en la barra lateral del complemento.

![Opción de historial de generación mostrada para un anuncio de Meta](./generation-history.png){width="80%" zoomable="yes"}

## Resolución de problemas

Tenga en cuenta estas prácticas recomendadas y sugerencias si el texto o las imágenes no se reemplazan en variaciones generadas.

### Campos asignados

Si no se reemplazan texto o imágenes, compruebe que los campos se hayan asignado a las funciones de campo de GenStudio en la interfaz de usuario del complemento. Consulte [Asignación de funciones de campo](#field-role-mapping).

### Confirmar fuentes disponibles

La fuente de un campo de texto debe estar disponible en el equipo para que el reemplazo se produzca durante la generación. Confirme que todas las fuentes utilizadas en el archivo están disponibles en el equipo, especialmente si el archivo se creó en el equipo de otra persona.

### Considerar compatibilidad con funciones de campo

Algunos canales solo admiten el reemplazo en campos específicos. Tenga en cuenta las excepciones para la asignación de funciones de [campo](#field-role-mapping).
