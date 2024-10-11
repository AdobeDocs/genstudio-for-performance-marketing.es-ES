---
title: Notas de la versión de Adobe GenStudio for Performance Marketing Beta
description: Obtenga información sobre las últimas funciones y mejoras de Adobe GenStudio for Performance Marketing.
hidefromtoc: true
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: 9b5e8b37ba988c3dd4a1e5a828487997375474ac
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# Notas de la versión de Adobe GenStudio for Performance Marketing Beta

En estas notas se destacan las correcciones y mejoras significativas realizadas en Adobe GenStudio for Performance Marketing durante la semana que finalizó el 4 de octubre.

## Nuevas funciones y mejoras

* Se ha mejorado la capacidad de filtrado en todo el producto. Se han resuelto los problemas con el filtrado por edad y sexo en [!DNL Insights].  <!-- GS-1198 -->

* Puede editar recursos de imagen (en formato de JPG o PNG) directamente mediante el Adobe Express. Los editores de contenido pueden usar el lienzo _[!UICONTROL Powered by Adobe Express]_ para quitar fondos, aplicar rellenos generativos, ajustar efectos y recortar imágenes sin salir de GenStudio for Performance Marketing. <!-- GS-4615 -->

* Se ha mejorado la experiencia de carga progresiva para variantes generadas, correo electrónico generado y mensajería contextual. <!-- GS-4651 3062-->

* Los editores de contenido ahora pueden utilizar la función de ajuste de recorte para recortar imágenes procesadas en variantes. <!-- GS-2342 -->

* Se han resuelto los problemas con el cambio de tamaño y la duplicación de plantillas. <!-- GS-4895 -->

* La validación de marca ahora explica la causa de los errores que se producen durante la validación.

* Las vistas previas de plantilla ahora muestran el texto en la imagen según lo esperado. <!-- GS-5917 -->

## Mejoras adicionales y problemas corregidos

* El lienzo [!DNL Create] ahora procesa fuentes personalizadas de plantillas según lo esperado. <!-- GS-3415 -->

* La fuente correcta ahora se aplica durante la exportación del anuncio Meta. <!-- GS-5875 -->

* Se han resuelto los problemas con la carga de plantillas que provocaban una carga correcta, pero que no tenían visibilidad en la interfaz del producto. <!-- GS-4815 5650-->

* Los usuarios ahora pueden recortar manualmente los anuncios Meta después de cambiar su tamaño. <!-- GS-5871 -->

* Los usuarios ya no tienen que iniciar sesión dos veces en una cuenta de Meta ads de canal cuando también inician sesión en Facebook. <!-- GS-3009 -->

* La vista de lienzo de los recursos y las experiencias ahora es coherente en todo el proceso de creación, revisión y aprobación de contenido. <!-- GS-5877 -->

* El lienzo ahora muestra solo cuatro variantes al regenerar después de una operación de cambio de tamaño. <!-- GS-5869 -->

* La revisión ortográfica basada en explorador ahora funciona según lo esperado en el lienzo [!DNL Create]. <!-- GS-5760 -->

* Los anuncios de visualización ahora se exportan como archivos PNG cuando se selecciona **[!UICONTROL Exportar como PNG]**. Anteriormente, los anuncios de visualización se exportaban como JPEG cuando se seleccionaba el formato PNG. <!-- GS-5545 -->

* Se ha aumentado el relleno entre el botón **[!UICONTROL Recorte manual]** y el botón **[!UICONTROL Generar]**. Anteriormente, el botón **[!UICONTROL Recorte manual]** estaba parcialmente oscurecido. <!-- GS-6084 -->

* Las previsualizaciones de plantilla ahora muestran las fuentes de Google según lo esperado. <!-- GS-5946 -->

* Las fuentes TypeKit y Google importadas ahora se cargan según lo esperado durante la exportación. <!-- GS-5948 -->

* Se han resuelto problemas con la generación de contenido con plantillas personalizadas. Anteriormente, cuando un editor de contenido intentaba generar un recurso mediante una plantilla personalizada, la ventana emergente de generación no se mostraba y la consola mostraba errores. <!-- GS-5262 -->

* El lienzo de borrador de DisplayAds ahora mantiene su posición cuando un usuario hace clic con el botón derecho en el lienzo antes de hacer clic con el botón izquierdo fuera del menú contextual. Anteriormente, el lienzo cambiaba cuando el usuario hacía clic con el botón izquierdo, lo que hacía que el contenido del borrador no fuera parcialmente accesible.  <!-- GS-5687 -->

* Los efectos de brillo de carga ahora persisten hasta que se completa la regeneración de la imagen.  <!-- GS-5811 -->

* Las puntuaciones de validación de marca ya no se invalidan después de que un usuario realice ediciones en correos electrónicos, anuncios Meta o anuncios en pantalla generados. Anteriormente, esta puntuación estaba oculta. <!-- GS-5379 -->

* Las plantillas que tienen estilos CSS adjuntos a su elemento `body` ahora se aprovechan como se espera durante la exportación de experiencias. <!-- GS-5947 -->

* Se han corregido problemas con el recorte manual de imágenes de gran dimensión. <!-- GS-6039 -->

* Ahora solo aparece un mensaje emergente cuando un usuario agrega un nuevo recurso en [!DNL Content]. <!-- GS-5020 -->

* Se ha mejorado el rendimiento del lienzo durante la edición de texto.  <!-- GS-5118 -->

* Se agregaron los espacios que faltaban entre cadenas en el correo electrónico [!DNL Create] o en el lienzo de metaanuncios. <!-- GS-5019 -->

* Los editores ahora pueden guardar un archivo con nombres que contengan caracteres especiales después de editarlo en Express. <!-- GS-6131 -->

### Localización

Esta versión incluye mejoras en la localización en toda la interfaz de producto, incluidas estas áreas de interfaz:

* Dirección URL del destino de la opción **[!UICONTROL Más información]** en el menú de [!DNL Create] mensajes. <!-- GS-5029 -->

* Formatos de número adyacentes a los campos de entrada de búsqueda [!DNL Insights] > [!DNL Experience]. <!-- GS-4494 -->

## Problema conocido

* Los fragmentos de correo electrónico regenerados no aparecen en la variante después de la selección. (Sin embargo, las variantes aparecen después de volver a abrir el borrador). <!-- GS-5913 -->
