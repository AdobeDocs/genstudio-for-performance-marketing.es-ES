---
title: 'Crear experiencia de anuncio de Meta: anuncios de carrusel'
description: Aprenda a crear experiencias de anuncios de carrusel de Meta de varias tarjetas, administrar tarjetas y generar conceptos de marca en [!DNL GenStudio for Performance Marketing].
role: User
source-git-commit: 1b407c1c66a2426b21cbbf423774ebdff16a7dec
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 1%
---

# Crear una experiencia de anuncio de carrusel de Meta

Un anuncio de carrusel de Meta es un formato de anuncio de pago que muestra de dos a diez tarjetas despegables, cada una con su propia imagen o vídeo, titular y vínculo.

Esta página cubre los pasos específicos de los anuncios de carrusel. Para ver los pasos compartidos que esta página no repite, como elegir una plantilla, agregar parámetros, revisar variantes y publicar, consulte [Crear una experiencia de anuncio de Meta](/help/user-guide/create/create-meta-ad.md).

## Requisitos previos

Antes de crear un anuncio de carrusel, asegúrese de tener una plantilla cuyas páginas compartan una relación de aspecto, ya sea 1:1 o 4:5. Cada página de plantilla se convierte en una tarjeta. Para obtener más información, consulte [Directrices para plantillas de anuncios de Meta](/help/user-guide/templates/meta-template.md).

## Elija el formato de carrusel

Después de seleccionar una plantilla y abrir el lienzo, elija el formato de carrusel en el cajón de mensajes.

1. En el panel _[!DNL Create your ads]_, expanda&#x200B;_[!UICONTROL &#x200B; Parámetros &#x200B;]_.
1. En el menú desplegable **[!UICONTROL Formato]**, seleccione **[!UICONTROL Carrusel y]**.

   ![El panel Crear tus anuncios con la lista desplegable Formato establecida en Anuncio de carrusel y una lista de tarjetas](./carousel-format-cards.png){width="70%" zoomable="yes"}

Si comienza desde una plantilla de una sola página, [!DNL GenStudio for Performance Marketing] duplica la página para alcanzar el mínimo de dos tarjetas. Si las páginas de la plantilla no comparten una proporción de aspecto, el cambio de formato se bloqueará hasta que utilice una plantilla con una proporción de aspecto coherente.

## Administración de tarjetas

Cree el conjunto de tarjetas en el cajón de mensajes antes de generar. Para agregar más tarjetas, duplique una tarjeta existente.

* **Para duplicar una tarjeta**, seleccione **[!UICONTROL Duplicar]** de las opciones de tarjeta.
* **Para reordenar las tarjetas**, arrastre una tarjeta por su controlador a una nueva posición.
* **Para eliminar una tarjeta**, seleccione **[!UICONTROL Eliminar]** de las opciones de tarjeta. Las dos últimas tarjetas no se pueden eliminar porque un carrusel requiere al menos dos tarjetas.

Para cada tarjeta, seleccione una imagen y, si es necesario, establezca un producto por tarjeta que anule el producto principal. Puede seleccionar una imagen por tarjeta de forma individual. Las direcciones URL de destino por tarjeta se establecen más adelante en [!DNL Activate]. Para obtener más información, consulte [Activar un anuncio de Meta](/help/user-guide/activation/activate-meta-ad.md).

## Escribir un mensaje de carrusel

El mensaje indica la intención del carrusel, por lo que debe describir cómo se relacionan las tarjetas entre sí. La copia de carrusel puede seguir uno de dos enfoques:

* **Modular:** Cada tarjeta es un anuncio independiente y no fluye ninguna copia entre las tarjetas. Utilice este método para un conjunto de mensajes relacionados pero independientes, como varios productos.
* **Secuencial:** la copia se conecta entre tarjetas para contar una historia, una secuencia paso a paso o un procedimiento. Utilice este método cuando las tarjetas se basen unas en otras.

También puede describir si el carrusel incluye un solo producto o varios, además de cualquier detalle por tarjeta.

Por ejemplo, este mensaje describe un carrusel modular que incluye varios productos:

```properties
Create a multi-product carousel for our end-of-summer skincare sale. For each card, lead with the product's core benefit and emphasize the sale value.
```

Este mensaje describe un carrusel secuencial que cuenta una historia en cinco tarjetas:

```properties
Create a narrative carousel for our compliance alert-management platform. Start with shared intro text about the cost of alert fatigue. Across five cards, build the story: rising review costs, too many low-value alerts, false positives as the hidden cost driver, a solution that cuts false positives by more than 50%, and a closing learn-more call to action.
```

Para ver los aspectos básicos de las peticiones, consulte [Escribir peticiones de datos efectivas](/help/user-guide/effective-prompts.md).

## Generar y revisar conceptos

Una vez configuradas las tarjetas y el indicador, genere el carrusel y revise los resultados.

1. Seleccione **[!UICONTROL Generar]**.

   [!DNL GenStudio for Performance Marketing] genera cuatro conceptos de carrusel. Cada concepto es un carrusel completo de varias tarjetas con su propia puntuación de marca.

   ![Cuatro conceptos de carrusel generados, cada uno con una puntuación de marca y un botón Editar](./carousel-concepts.png){width="80%" zoomable="yes"}

1. Seleccione un concepto y, a continuación, seleccione **[!UICONTROL Editar]** para abrirlo y editarlo.
1. Usa las flechas para moverte entre tarjetas, luego edita el texto o selecciona **[!UICONTROL Intercambiar]** para cambiar la imagen de una tarjeta. Para obtener más información sobre la edición, consulte [Administrar variantes](/help/user-guide/create/manage-variants.md).

Si reordena las tarjetas antes de generarlas, el lienzo se actualiza inmediatamente. Si reordena las tarjetas en el cajón de solicitud después de generar, el cambio solo se aplicará después de volver a generar y aparecerá una advertencia de regeneración.

## Comprender los campos compartidos y por tarjeta

Algunos campos de carrusel se aplican a cada tarjeta individualmente y otros se aplican a todo el anuncio. En la tabla siguiente se describe cómo se comporta cada campo para los anuncios de carrusel de Meta.

| Campo | Ámbito |
|---|---|
| Titular | Por tarjeta |
| Descripción | Por tarjeta, opcional, establecida en [!DNL Activate] |
| Call to action | Compartido en el anuncio |
| Texto principal | Compartido en el anuncio |
| Medios | Por tarjeta (imagen, vídeo o mixto) |
| Texto en la imagen | Por tarjeta |
| URL de destino | Por tarjeta, establecida en [!DNL Activate] |

## Publicación, exportación y activación

Cuando el carrusel esté listo, publíquelo y exporte del mismo modo que para otros anuncios de Meta. Un carrusel se almacena como una experiencia única que corresponde a un concepto. La exportación envía un archivo CSV más los medios de la tarjeta. Consulte [[!DNL Content]](/help/user-guide/content/overview.md) para ver cómo se almacenan las experiencias publicadas. Para activar tu carrusel en Meta, consulta [Activar un anuncio de Meta](/help/user-guide/activation/activate-meta-ad.md).
