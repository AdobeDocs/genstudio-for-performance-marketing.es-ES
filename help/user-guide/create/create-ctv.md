---
title: Crear una experiencia de TV conectada
description: Aprenda a crear anuncios de TV (CTV) conectados en Adobe [!DNL GenStudio for Performance Marketing], desde informes y recursos hasta generación, edición de escenas, revisión y exportación.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
source-git-commit: 513ad53218828f154cdf13a8ae42f3bd94b5546d
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 1%

---


# Crear una experiencia de TV conectada

Use [[!DNL Create]](/help/user-guide/create/overview.md) en [!DNL GenStudio for Performance Marketing] para generar anuncios de TV (CTV) conectados en un solo lugar, desde instrucciones breves y compartidas hasta la generación, el refinamiento basado en escenas, la aprobación y la exportación lista para el editor. El flujo de trabajo siguiente se ejecuta por completo en [!DNL GenStudio for Performance Marketing]; no hay ninguna aplicación CTV independiente ni incrustación de editor.

## Requisitos previos

Antes de crear un anuncio de CTV, confirme lo siguiente:

* Acceso a [!DNL GenStudio for Performance Marketing].
* **[!DNL Brands]**, **[!DNL Products]** y **[!DNL Personas]** se configuraron como objetos compartidos en [!DNL GenStudio for Performance Marketing]. Consulte [Información general sobre las directrices](/help/user-guide/guidelines/overview.md) para comprender cómo informan estos objetos a la generación.
* Se recomiendan los recursos de la campaña (clips de vídeo, imágenes, logotipos, música), pero no son necesarios. La IA generativa puede rellenar huecos cuando faltan recursos o están incompletos.

## Crear nuevo anuncio de CTV

Todo en este flujo de trabajo sucede dentro de [!DNL GenStudio for Performance Marketing].

![Tarjeta de creación de TV conectada](./ctv-tile.png){width="50%"}
**Para navegar a la creación de CTV**:

1. Iniciar sesión en [!DNL GenStudio for Performance Marketing].
1. Desde la superficie de inicio o creación, ve a **[!UICONTROL Crear]**.
1. Seleccione **CTV** mediante la tarjeta de creación de CTV.
1. Haga clic en **[!UICONTROL Crear anuncio de CTV]**.

Se abre una experiencia de creación de CTV única y optimizada. No es necesario que elija primero un tipo de anuncio.

## Configuración de la información

Las instrucciones y las entradas impulsan la forma en que se genera el anuncio. Esta es su oportunidad para proporcionar contexto y restricciones para el proceso de generación de anuncios.

![Configurar la información](./ctv-brief.png){width=80%&quot; align=&quot;center&quot;}

**Para configurar el informe**:

1. Seleccione **[!DNL Brands]**, **[!DNL Products]** y **[!DNL Personas]** de los objetos compartidos existentes.
1. Agregue **informe creativo** introduciéndolo directamente o cargándolo. Incluya el objetivo de la campaña, el mensaje clave y cualquier restricción.
1. Establezca **duración del anuncio** en 15 o 30 segundos.
1. Opcionalmente, agregue **recursos**. Cargue clips de vídeo, imágenes, logotipos, música, voz en off o tarjetas de introducción y salida (arrastre y suelte o seleccione un archivo), o bien elija recursos de su repositorio de [!DNL Content].
1. Haga clic en el botón **[!UICONTROL Generar]**.

Si los recursos faltan o están incompletos, [!DNL GenStudio for Performance Marketing] puede generar escenas, música o voz en off que faltan mediante IA. Assets que proporcione siempre tendrá prioridad sobre el material generado.

[!DNL GenStudio for Performance Marketing] automáticamente:

* Interpreta el informe junto con el contexto de **[!DNL Brands]**, **[!DNL Products]** y **[!DNL Personas]**.
* Agrupa una estructura de anuncios CTV completa.
* Crea escenas, superposiciones de texto, música y voz en off según sea necesario.
* Aplica duración y formato compatibles con CTV.

El resultado es un anuncio de CTV completamente formado y con vista previa, no una cronología de borrador.

## Editar y perfeccionar la publicidad

Utilice el editor basado en escenas para refinar el anuncio sin regenerarlo todo.

Haga clic en una escena de la franja de escenas para abrirla y editarla. Las ediciones que puede realizar incluyen:

* Reemplace o vuelva a generar una sola escena con IA.
* Edite el indicador de escena para crear variantes.
* Reordenar o recortar escenas.
* Editar superposiciones de texto.
* Intercambia, silencia o reemplaza música y voz en off.
* Ajuste las transiciones entre escenas.

La edición está diseñada para que pueda regenerar una escena a la vez para una iteración más rápida y una actualización creativa.

>[!NOTE]
>
>El editor no admite el cambio de objetos *dentro* de un clip de vídeo (por ejemplo, quitar elementos, cambiar colores de productos o modificar el aspecto de las personas).

## Revisar y aprobar

Envíe el anuncio para su revisión de marca mediante los flujos de trabajo de aprobación integrados. Los revisores de marcas y partes interesadas comprueban la mensajería, los elementos visuales y el cumplimiento de la marca. Los aprobadores validan el anuncio; no se espera que realicen edición de vídeo en lugar del experto en marketing.

## Exportar

Después de la aprobación, puede:

* Exporte el anuncio CTV finalizado en un formato compatible y listo para su publicación.
* Vuelva a guardar el anuncio en [!DNL Content].
* Utilícelo en flujos de trabajo de compra y tráfico de CTV descendentes.

Creative está diseñado para estar listo para la activación sin volver a codificar ni volver a trabajar.
