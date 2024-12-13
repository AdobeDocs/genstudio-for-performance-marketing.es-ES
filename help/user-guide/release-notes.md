---
title: Notas de la versión de Adobe GenStudio for Performance Marketing
description: Obtenga información sobre las últimas funciones y mejoras de Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
last-substantial-update: 2024-12-13T00:00:00Z
exl-id: 32f5104e-ae15-4092-8a34-642fc641baf9
source-git-commit: 00359960b6cf314203382d74faa23bae3e753875
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 1%

---

# Notas de la versión de GenStudio for Performance Marketing

Esta información de la versión detalla las últimas actualizaciones de la aplicación de GenStudio for Performance Marketing.

## 2024.12.12 {#latest}

### Nuevas funciones

Los editores ahora pueden realizar las siguientes tareas relacionadas con los metadatos:

* Editar metadatos de recursos, experiencias y plantillas. Ver [detalles del recurso](/help/user-guide/content/asset-details.md#user-defined-metadata). <!-- GS-4905 6935-->

* Vea las etiquetas generadas por un recurso en la vista _Detalles_ de cualquier experiencia que utilice el recurso. Ver _etiquetas generadas_ en [detalles del recurso](/help/user-guide/content/asset-details.md#generated-tags). <!-- GS-3705 -->

Los editores ahora pueden especificar valores personalizados para estos aspectos de las variantes generadas:

* Anchura y altura de los titulares web en las plantillas de anuncios en pantalla. Estos valores ahora se guardan como metadatos de plantilla. <!-- GS-6735 -->

* Dimension a imágenes en experiencias de anuncios en pantalla durante la carga de imágenes.<!-- GS-7166 -->

* Consulte las directrices específicas del canal en las [Prácticas recomendadas para plantillas](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines).

Las opciones de exportación ahora incluyen:

* Exporte anuncios en pantalla y anuncios Meta como HTML, JPEG o PNG. Ver [Crear una experiencia de anuncio en pantalla](/help/user-guide/create/create-display-ad.md) y [Crear una experiencia de anuncio meta](/help/user-guide/create/create-meta-ad.md). <!-- GS-7093 6655 5152-->

Las nuevas funciones adicionales permiten a los editores:

* Use el botón **[!UICONTROL Actualizar]** de la vista _Detalles del recurso_ de la plantilla [!DNL Content] para actualizar la plantilla seleccionada. <!-- GS-7102 -->

* Regenerar secciones de anuncios en pantalla y variantes de correo electrónico. Ver [Crear una experiencia de anuncio en pantalla](/help/user-guide/create/create-display-ad.md#revise-generated-display-ads) y [Crear una experiencia de correo electrónico](/help/user-guide/create/create-email-experience.md#revise-generated-emails). <!-- GS-5080 5078-->

* Duplicar marcas existentes. Ver [Administrar marcas](/help/user-guide/guidelines/brands.md#manage-brands). <!-- BRANDS-548 -->

### Correcciones y mejoras

* Los títulos de anuncios de visualización ahora se han guardado en [!DNL Content] según lo esperado. <!-- GS-7239 -->

* El cajón de mensajes ya no se cierra cuando un editor hace clic fuera del menú desplegable del cajón. <!-- GS-7275 -->

* El menú desplegable [!DNL Create] [!DNL Persona]/[!DNL Product] ahora se carga según lo esperado cuando se produce un error en el servicio de URL en miniatura. <!-- GS-7277 -->

* Los anuncios de visualización que contienen elementos que se superponen a fragmentos ahora se pueden editar. <!-- GS-7186 -->

* El botón Lienzo **[!UICONTROL Marca]** ahora está deshabilitado cuando las puntuaciones de marca no se generan para una experiencia. <!-- GS-6429 -->

* El lienzo ahora muestra las experiencias cuyo tamaño se ha cambiado en orden coherente. <!-- GS-7123 -->

* El recorte manual ahora utiliza dimensiones de imagen, no dimensiones de plantilla, al editar anuncios en pantalla. Anteriormente, cuando una imagen era más pequeña que las dimensiones especificadas en la plantilla de anuncio de visualización, el cuadro delimitador utilizaba dimensiones de plantilla, no dimensiones de imagen. <!-- GS-7315 -->

* Los editores ahora pueden seleccionar hasta cuatro imágenes al crear un anuncio en pantalla. <!-- GS-7189 -->

* Los borradores de anuncios de display y Meta ahora se cargan según lo esperado al cambiar el tamaño en un explorador diferente. <!-- GS-7204 -->

* Los campos de plantilla no utilizados ya no se muestran en el contenido generado.  <!-- GS-5670 -->

* Los editores ahora pueden hacer clic en los vínculos para editarlos como se espera en las variantes generadas. <!-- GS-7423 -->

* [!DNL Create] ahora respeta correctamente los privilegios de colaborador. <!-- GS-7614 -->

* El botón **[!UICONTROL Cambiar tamaño]** del lienzo ahora está deshabilitado después de seleccionar y procesar todas las opciones de cambio de tamaño. <!-- GS-5940 -->

* Los revisores con acceso de solo vista ahora pueden acercar y alejar las variantes durante las revisiones. <!-- GS-7371 -->

* El foco del teclado se ha agregado únicamente a los botones de acción de la vista [!DNL Create] _Trabajo reciente_. <!-- GS-4060 -->

* El mensaje **Guardar en curso** que se muestra durante las operaciones de guardado de fragmentos de correo electrónico ahora solo se muestra durante la operación de guardado. Anteriormente, el lienzo mostraba este mensaje indefinidamente. <!-- GS-6964 -->

* Los editores ahora ven un mensaje de error como se espera cuando un borrador no se puede cargar en el área [!DNL Create] _Trabajo reciente_.  <!-- GS-8081 -->

* El lienzo ahora muestra los anuncios Meta redimensionados y los anuncios de visualización en el orden correcto.  <!-- GS-7375 -->

* Los editores ahora pueden hacer clic en los campos del correo electrónico y mostrar anuncios. <!-- GS-6297 -->

* La capacidad Editar fragmento para anuncios Meta y de correo electrónico ahora se activa como se espera con un solo clic. <!-- GS-8081 -->

* Se mejoró el rendimiento del botón [!DNL Create] **[!UICONTROL Atrás]**. <!-- GS-6767 -->

## Notas de la versión anteriores

+++Notas de 2024.11.14

### Nuevas funciones

Se ha agregado compatibilidad con las plantillas de medios enriquecidos, lo que permite a los clientes reutilizar recursos que ya se han publicado a través de sus propios canales de contenido administrado. <!-- GS-6107 -->

### Correcciones y mejoras

* Cuando se cambia el tamaño en un explorador que no sea el utilizado para generar el contenido inicial, los borradores ahora se cargan según lo esperado. <!-- GS-7204 -->

* Ahora todos los caracteres se representan correctamente en el HTML exportado. <!-- GS-7246 -->

* Los botones de la ventana emergente [!DNL Content] _Experiencias_ **[!UICONTROL Exportar]** ya no están truncados en algunos idiomas. <!-- GS-6873 -->

* Los anuncios de visualización creados con plantillas de tamaño 50 x 50 ahora se exportan con el tamaño de imagen esperado. Anteriormente, los archivos PNG se exportaban al doble de las dimensiones esperadas. <!-- GS-7192 -->

* Los errores de plantilla que se producían cuando se cambió el tamaño de los anuncios de visualización ahora se resuelven. <!-- GS-7322 -->

### Localización

Esta versión incluye mejoras en la localización en toda la interfaz de usuario, como:

* Todas las cadenas de la ventana emergente [!DNL Content] _Cargar recurso_ se han localizado correctamente. <!-- GS-6872 6770 -->
* Todas las informaciones de herramientas del campo [!DNL Content] _Assets_ vista **[!UICONTROL Buscar]** están localizadas. <!-- GS-6879 -->
* Al reemplazar una imagen existente en una variante de correo electrónico en el lienzo [!DNL Create], la vista _Seleccionar del contenido_ ahora está localizada. <!-- GS-6906 -->

+++

+++Notas de la versión 2024.11.07

### Correcciones y mejoras

* El control de número _Guardar en curso_ ya no se muestra cuando un usuario hace clic en **[!UICONTROL Cargar nueva imagen]** y cancela la operación antes de que se complete la carga. <!-- GS-6780 -->

* Los títulos de las experiencias ahora se crean correctamente durante la regeneración de la experiencia. <!-- GS-7006 -->

* Se han resuelto los problemas con las barras de desplazamiento parpadeantes durante la carga del borrador. <!-- GS-5587 -->

* El vínculo `View documentation` en la ventana emergente [!DNL Content] _Agregar la plantilla aprobada_ funciona ahora según lo esperado. <!-- GS-6881 -->

* La eliminación de una imagen del cajón de mensajes durante una operación de cambio de tamaño ya no provoca un error. <!-- GS-7115 7009 -->

* Ahora, seleccionar **[!UICONTROL Eliminar]** del menú de acción [!DNL Create] (...) funciona según lo esperado. <!-- GS-6871 -->

* Ahora los usuarios pueden controlar todos los elementos interactivos de las plantillas de publicidad Meta mediante el teclado. <!-- GS-4066 -->

* Se ha añadido la extracción de dimensiones de imagen de los campos de imagen de plantilla a las plantillas de anuncio de visualización. Las solicitudes de recorte inteligente ahora se envían para la dimensión real de la imagen y no para toda la plantilla. <!-- GS-6926 -->

* Se localizó la cadena `Zoom to fit to screen` en el correo electrónico y los anuncios Meta generados. <!-- GS-5063 -->

* El cajón de mensajes [!DNL Create] ahora se cierra como se espera cuando un usuario hace clic fuera. <!-- GS-5254 -->

* La exportación de meta-ads ahora incluye la etiqueta de llamada a la acción seleccionada según lo esperado. <!-- GS-6504 -->

* La puntuación de la marca ahora se actualiza y se conserva según lo esperado para las experiencias regeneradas. <!-- GS-6535 -->

* La exportación de HTML de anuncios Meta y anuncios de visualización ya no incluye los elementos envolvente `div` y `chrome`. <!-- GS-7116 -->

* Ya se han resuelto los problemas con el procesamiento del borrador de correo electrónico durante la publicación. <!-- GS-6394 -->

* El botón Lienzo **[!UICONTROL Marca]** ahora está deshabilitado cuando no se genera una puntuación de marca. <!-- GS-6429 -->

* El conmutador Facebook/Instagram de la barra de acciones Lienzo ahora actualiza las representaciones de experiencias como se espera cuando la configuración Lienzo `ReadOnly` está habilitada. <!-- GS-7039 -->

#### Regeneración de imagen

* Ahora, cambiar el tamaño de varias variantes de MetaAd funciona según lo esperado. Anteriormente, el lienzo no mostraba variantes regeneradas, pero permanecía en blanco. <!-- GS-7010 -->

* La regeneración de fragmentos ahora funciona según lo esperado para las experiencias cuyo tamaño se ha cambiado. <!-- GS-6836 -->

* La regeneración de las imágenes de Meta y Ad después de cambiar su tamaño ya no provoca un error. Anteriormente, el cambio de tamaño de las imágenes antes de la regeneración cambió los metadatos de canal de `meta` a `facebook`. <!-- GS-7042 -->

+++

+++Notas de 2024.10.31

### Nuevas funciones

* El filtro de búsqueda **[!DNL Content]** ahora admite la búsqueda por etiqueta de color. <!-- GS-5501 -->

* El lienzo **[!DNL Create]** ahora muestra recuentos de caracteres para los fragmentos de correo electrónico. <!-- GS-5819 -->

### Correcciones y mejoras

* Se han agregado las etiquetas de lector de pantalla que faltan a los elementos del móvil y del escritorio `view`. <!-- GS-5624 4729 -->

* Las áreas de línea de asunto y texto previo al encabezado del correo electrónico de lienzo **[!DNL Create]** ahora son dinámicas en altura. <!-- GS-6258 -->

* Se han resuelto los problemas de diseño con los bordes de correo electrónico. <!-- GS-6631 -->

* Ahora, el foco del teclado funciona según lo esperado en el botón **[!DNL Content]** **[!UICONTROL Eliminar]**. Anteriormente, los usuarios no podían acceder a este botón mediante el teclado.  <!-- GS-4065 -->

+++

+++Notas de la versión 2024.10.14 Disponibilidad general

Esta versión presenta Adobe GenStudio for Performance Marketing, una aplicación generativa basada en IA que acelera la planificación, el desarrollo y el análisis de las campañas de marketing. GenStudio for Performance Marketing permite a los equipos de marketing crear contenido multicanal y de marca para anuncios, correos electrónicos y campañas, a la vez que proporciona perspectivas en tiempo real para optimizar el rendimiento del contenido.

### Funciones

Las principales funciones del producto incluyen:

**[!DNL Create]** presenta el lienzo, que ofrece una experiencia de mensaje estructurada que permite a los editores de contenido generar rápidamente contenido y variantes. Los administradores de sistemas entrenan el producto en directrices de marca organizativas. [!DNL Create] garantiza que todo el contenido generado por IA se ajuste a las directrices de marca (marca, perfiles de clientes y descripciones de productos) y optimiza la producción de contenido de marketing de alto impacto y coherente con la marca.

**[!DNL Content]** almacena recursos y experiencias aprobados seleccionados y compatibles con la marca. Los usuarios de GenStudio for Performance Marketing pueden encontrar, editar, reutilizar y compartir fácilmente los recursos aprobados, lo que reduce la necesidad de volver a crear contenido desde cero para cada campaña.

**[!DNL Reviews and Approvals]** establece un marco de trabajo para que las partes interesadas revisen y aprueben las variantes generadas antes de guardarlas en **[!DNL Content]** o exportarlas.

**[!DNL Campaigns]** organiza y administra las campañas de marketing para garantizar una ejecución y un seguimiento optimizados. Los colaboradores pueden visualizar, planificar y realizar un seguimiento de las campañas para administrar varias iniciativas de forma eficaz y garantizar una entrega puntual.

**[!DNL Insights]** ofrece una evaluación en tiempo real del rendimiento del contenido, lo que ayuda a los especialistas en marketing a optimizar sus estrategias y tomar decisiones basadas en datos.

GenStudio for Performance Marketing se integra con otros productos de Adobe Experience Cloud, incluidos los AEM Assets de Adobe Express y Adobe.

+++
