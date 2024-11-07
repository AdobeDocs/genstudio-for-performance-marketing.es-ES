---
title: Notas de la versión de Adobe GenStudio for Performance Marketing
description: Obtenga información sobre las últimas funciones y mejoras de Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
source-git-commit: b502e0a558cbc26c70d813938734a2f6f230dc8e
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 3%

---

# Notas de la versión de GenStudio for Performance Marketing

Esta información de la versión detalla las últimas actualizaciones de la aplicación de GenStudio for Performance Marketing.

## 2024.11.07 {#latest}

### Correcciones

* El control de número _Guardar en curso_ ya no se muestra cuando un usuario hace clic en **[!UICONTROL Cargar nueva imagen]** y cancela la operación antes de que se complete la carga. <!-- GS-6780 -->

* Los títulos de las experiencias ahora se crean correctamente durante la regeneración de la experiencia. <!-- GS-7006 -->

* Se han resuelto los problemas con las barras de desplazamiento parpadeantes durante la carga del borrador. <!-- GS-5587 -->

* El vínculo `View documentation` en la ventana emergente [!DNL Content] _Agregar la plantilla aprobada_ funciona ahora según lo esperado. <!-- GS-6881 -->

* La eliminación de una imagen del cajón de mensajes durante una operación de cambio de tamaño ya no provoca un error. <!-- GS-7115 7009 -->

* Ahora, seleccionar **[!UICONTROL Eliminar]** del menú de acción [!DNL Create] (...) funciona según lo esperado. <!-- GS-6871 -->

* Ahora los usuarios pueden controlar todos los elementos interactivos de las plantillas de publicidad Meta mediante el teclado. <!-- GS-4066 -->

* Se ha añadido la extracción de dimensiones de imagen de campos de imagen de plantilla para mostrar plantillas de anuncios. Las solicitudes de recorte inteligente ahora se envían para la dimensión real de la imagen y no para toda la plantilla. <!-- GS-6926 -->

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

## 2024.10.31

### Nuevas funciones

* El filtro de búsqueda **[!DNL Content]** ahora admite la búsqueda por etiqueta de color. <!-- GS-5501 -->

* El lienzo **[!DNL Create]** ahora muestra recuentos de caracteres para los fragmentos de correo electrónico. <!-- GS-5819 -->

### Correcciones

* Se han agregado las etiquetas de lector de pantalla que faltan a los elementos del móvil y del escritorio `view`. <!-- GS-5624 4729 -->

* Las áreas de línea de asunto y texto previo al encabezado del correo electrónico de lienzo **[!DNL Create]** ahora son dinámicas en altura. <!-- GS-6258 -->

* Se han resuelto los problemas de diseño con los bordes de correo electrónico. <!-- GS-6631 -->

* Ahora, el foco del teclado funciona según lo esperado en el botón **[!DNL Content]** **[!UICONTROL Eliminar]**. Anteriormente, este botón no se podía alcanzar ni utilizar mediante el teclado.  <!-- GS-4065 -->

## Versión de disponibilidad general 2024.10.14

Esta versión presenta Adobe GenStudio for Performance Marketing, una aplicación generativa basada en IA que acelera la planificación, el desarrollo y el análisis de las campañas de marketing. GenStudio for Performance Marketing permite a los equipos de marketing crear contenido multicanal y de marca para anuncios, correos electrónicos y campañas, a la vez que proporciona perspectivas en tiempo real para optimizar el rendimiento del contenido.

### Características

Las principales funciones del producto incluyen:

**[!DNL Create]** presenta el lienzo, que ofrece una experiencia de mensaje estructurada que permite a los editores de contenido generar rápidamente contenido y variantes. Los administradores de sistemas entrenan el producto en directrices de marca organizativas. [!DNL Create] garantiza que todo el contenido generado por IA se ajuste a las directrices de marca (promoción de la marca, perfiles de clientes y descripciones de productos) y optimiza la producción de contenido de marketing de alto impacto y coherente con la marca.

**[!DNL Content]** almacena recursos y experiencias aprobados seleccionados y compatibles con la marca. Los usuarios de GenStudio for Performance Marketing pueden encontrar, editar, reutilizar y compartir fácilmente los recursos aprobados, lo que reduce la necesidad de volver a crear contenido desde cero para cada campaña.

**[!DNL Reviews and Approvals]** establece un marco de trabajo para que las partes interesadas revisen y aprueben las variantes generadas antes de guardarlas en **[!DNL Content]** o exportarlas.

**[!DNL Campaigns]** organiza y administra las campañas de marketing para garantizar una ejecución y un seguimiento optimizados. Los colaboradores pueden visualizar, planificar y realizar un seguimiento de las campañas para administrar varias iniciativas de forma eficaz y garantizar una entrega puntual.

**[!DNL Insights]** ofrece una evaluación en tiempo real del rendimiento del contenido, lo que ayuda a los especialistas en marketing a optimizar sus estrategias y tomar decisiones basadas en datos.

GenStudio for Performance Marketing se integra con otros productos de Adobe Experience Cloud, incluidos los AEM Assets de Adobe Express y Adobe.

### Más información

Consulte los siguientes recursos útiles:

* [Guía del usuario de Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio/user-guide/home)

* [Academia de Adobe GenStudio](genstudioacademy.md), la plataforma de aprendizaje en línea de Adobe para usar tecnologías de IA generativa en el proceso creativo. [Regístrese en GenStudio Academy](http://adobe.ly/genstudioacademyregistration).
