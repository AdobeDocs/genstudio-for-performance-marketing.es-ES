---
title: Generar y refinar contenido con generación con estado
description: Aprenda a generar contenido propio de una marca y a refinarlo paso a paso en una conversación con voz impresa y señales visuales en [!DNL GenStudio for Performance Marketing].
feature: Create Prompt, Generative AI, Content Generation
role: User
level: Beginner
source-git-commit: 22db02c07a9f33cb1c70df9286ad6eb143dafd38
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%
---
# Generar y refinar contenido con generación con estado

[!DNL GenStudio for Performance Marketing] usa la generación con estado para ayudarle a crear contenido sin marca y, a continuación, refinarlo, paso a paso en una conversación, en lugar de empezar de nuevo con una nueva solicitud cada vez. A medida que perfecciona, la generación recuerda las instrucciones anteriores y las variantes que mantiene y, a continuación, aplica únicamente el cambio que solicita.

La generación con estado agrega tres tipos de contexto a las generaciones: la impresión de voz mantiene la copia en la voz de la marca, las indicaciones visuales son copia terrestre en una imagen o vídeo y la dirección URL de una página web agrega contexto de referencia desde una página que elija.

## Generación y refinamiento de contenido

1. En [!DNL GenStudio for Performance Marketing], inicie una generación para su canal y formato. Vea la [[!DNL Create] descripción general](/help/user-guide/create/overview.md) para comenzar una generación para cada canal.
1. _Opcional_: para poner la copia en su propio elemento creativo, seleccione **[!UICONTROL Seleccionar del contenido]** y, a continuación, elija una imagen o un vídeo para usar como [señal visual](#ground-content-in-an-image-or-video).
1. Seleccione **[!UICONTROL Generar]**. [!DNL GenStudio for Performance Marketing] crea un conjunto de variantes y aplica la [voz de marca](#keep-copy-in-your-brand-voice) automáticamente en los canales compatibles.
1. Restrinja los resultados en el cajón de mensajes. Escriba el cambio que desee, como `shorten the headline`, `make variant 2 punchier` o `change the headline`. La generación solo aplica ese cambio y mantiene las instrucciones anteriores.
1. Para conservar una variante mientras continúa perfeccionando, escriba una instrucción en el cajón de mensajes, como `keep variant 2`.
1. Cuando el contenido esté listo, exporte el contenido o envíelo para su revisión.

## Contenido terrestre en una imagen o un vídeo

Las indicaciones visuales permiten que la generación lea una imagen o un vídeo que adjunte y, a continuación, escriba una copia que refleje ese elemento creativo. La opción **[!UICONTROL Creative options]** controla las indicaciones visuales y está activada de forma predeterminada.

Para usar una señal visual, selecciona **[!UICONTROL Seleccionar del contenido]** y elige una imagen o un vídeo antes de generar. Para generar sin una señal visual, desactive **[!UICONTROL opciones de Creative]**.

>[!NOTE]
>Las indicaciones visuales no están disponibles para anuncios en pantalla de varios fotogramas o anuncios de carrusel.

## Mantenga una copia en la voz de su marca

La impresión de voz aplica la voz aprendida de la marca a la copia generada, de modo que suene dentro de la marca sin una solicitud adicional. Está activado de forma predeterminada para los canales que tienen [Insights](/help/user-guide/insights/overview.md), como LinkedIn y Meta.

## Uso de una página web como contexto

Puede dirigir la generación a una página web y utilizar su contenido como contexto. En el cajón de mensajes, escriba una instrucción que incluya la dirección URL, como `Use this URL to generate an ad for this channel: https://www.example.com`.

>[!NOTE]
>Introduzca la dirección URL en el mensaje. No lo agregue mediante _Parameters_.

## Funciones relacionadas

- [Administrar variantes](/help/user-guide/create/manage-variants.md): edita y ajusta las variantes generadas directamente en el lienzo.
- [Escriba mensajes efectivos](/help/user-guide/effective-prompts.md): Envíe mensajes personalizados que produzcan mejores resultados.
