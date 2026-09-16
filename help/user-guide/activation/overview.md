---
title: Información general de Activate
description: Obtenga información sobre cómo activar contenido con Adobe CX Enterprise y aplicaciones de terceros.
level: Beginner
feature: Ad Activation
exl-id: 365fe253-d189-467e-a723-f54cd74ff60b
TQID: https://experienceleague.adobe.com/-Nal0YqjTzKw4g2SM3IuMf0a13e87CWdTqBZPd0dBkU
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: d87258a7-722c-4afd-b632-adddc447c7aa
    internal-label: Ad activation
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%
---
# Activar Adobe GenStudio for Performance Marketing

En GenStudio for Performance Marketing [!DNL Activate] es donde se preparan y envían experiencias publicitarias a canales de publicidad de pago, como Meta o LinkedIn. _Activation_ toma una experiencia de anuncio aprobada y sus recursos, aplica la configuración que requiere un canal específico y luego la envía directamente a ese canal en un estado inactivo y desactivado. A partir de ahí, puede realizar una revisión final en el administrador de anuncios del canal antes de que su anuncio se publique.

[!DNL Activate] envía la experiencia directamente al canal, por lo que no es necesario exportar archivos ni cargarlos manualmente en el administrador de anuncios del canal.

Un administrador del sistema o editor de GenStudio debe conectar la cuenta de publicidad de cada canal de publicidad de pago para poder activar una experiencia de publicidad en ese canal.

## Activar funciones

Use [!DNL Activate] para preparar experiencias publicitarias para sus canales de anuncios pagados de destinatario. [Activar experiencias de forma masiva](create-activation.md) en varios canales de publicidad pagada en una sola tabla de activación. A continuación, [administra tus activaciones](manage-activations.md) para ver el estado y los detalles de cada experiencia activada.

>[!VIDEO](https://video.tv.adobe.com/v/3503538?learn=on)

### Activar experiencias aprobadas desde el contenido

Seleccione una o más experiencias aprobadas y publicadas de [!DNL Content], o comience desde la página de aterrizaje [!DNL Activate]. A diferencia de las versiones anteriores de [!DNL Activate], una sola tabla de activación puede incluir experiencias para varios canales de publicidad de pago a la vez, organizados por formato de anuncio y canal.

>[!NOTE]
>
>[!DNL Content] llama a un destino como Meta o LinkedIn en un **canal**. [!DNL Activate] llama al mismo destino que **platform** (por ejemplo, en **[!UICONTROL Platform setup]**). Los dos términos hacen referencia a la misma cosa.

### Configuración de los detalles de configuración de publicidad y plataforma

Cada fila de la tabla de activación representa un anuncio. Los recursos creativos, los titulares y las copias de cuerpo aprobados están bloqueados porque ya han pasado por la revisión y la aprobación. Puede editar los campos restantes, como el texto de call-to-action, la dirección URL de destino y los detalles de configuración de la plataforma, como la cuenta de publicidad, la campaña y el conjunto de anuncios. Edite los campos de una fila a la vez o seleccione varias filas para editar los campos compartidos de forma masiva.

### Revise y publique sus experiencias en sus canales publicitarios

Confirme que cada fila muestre [!UICONTROL Listo para activar]. [!DNL Activate] marca campos que faltan o no son válidos, llamadas a la acción incompatibles e ID de seguimiento duplicados como [!UICONTROL Necesita atención]. Cuando cada fila esté lista, haga clic en **[!UICONTROL Enviar a la plataforma]** para publicar todos los anuncios de la tabla. [!DNL Activate] informa del estado de cada anuncio en tiempo casi real, y los anuncios publicados correctamente incluyen un vínculo profundo al anuncio en el administrador de anuncios nativo de la plataforma de destino. Los anuncios fallidos devuelven un mensaje de error y se pueden volver a intentar.
