---
title: Administrar activaciones
description: Obtenga información sobre cómo administrar experiencias activadas con Adobe GenStudio for Performance Marketing.
feature: Ad Activation
exl-id: 7cf340d4-37ab-4906-9aad-088a26db0818
TQID: https://experienceleague.adobe.com/ird0IiW8L5Axjj2FmEjlUcD1sPaNCNfxj9XNqGfQWiI
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%
---
# Administración de activaciones

Las tablas de activación aparecerán en la página de aterrizaje [!DNL Activate]. Cada tabla enumera sus anuncios, junto con su estado:

| Estado | Significado |
|---|---|
| [!UICONTROL Necesita atención] | Al menos un anuncio de la tabla de activación tiene un campo que falta o no es válido, como un call to action incompatible o un ID de seguimiento duplicado. |
| [!UICONTROL Listo para activar] | Todos los anuncios de la tabla de activación superan la validación y están listos para publicarse. |
| [!UICONTROL Pendiente] | Se envió toda la tabla de activación y la plataforma de destino la está procesando. |
| [!UICONTROL Publicado] | Toda la tabla de activación se ha publicado correctamente. |
| [!UICONTROL Error] | La plataforma de destino rechazó al menos uno de los anuncios de la tabla. Pase el ratón sobre la información del estado para ver el mensaje de error de la plataforma. |

Para reintentar automáticamente las activaciones fallidas, haz clic en **[!UICONTROL Intentar de nuevo]** en la parte superior derecha.

Las filas publicadas no se pueden volver a enviar e incluyen un vínculo profundo al anuncio en el administrador de anuncios nativo de la plataforma de destino, por lo que puede ir directamente a él para revisarlo o iniciarlo.

## Vista de detalles

Haga clic en una fila de anuncio para abrir una vista enfocada de los detalles de activación. La vista de detalles de solo lectura captura los detalles de definición de un anuncio activado, incluidas las activaciones fallidas, con información derivada tanto de GenStudio for Performance Marketing como de la plataforma de destino:

* **Fecha y hora de publicación**: Fecha y hora de publicación desde la plataforma de destino
* **ID de anuncio**: ID asignado por la plataforma de destino y utilizado para el seguimiento, con un vínculo profundo al anuncio publicado en el administrador de anuncios nativo de la plataforma
* **Detalles del anuncio**: Los recursos, copias y metadatos aprobados utilizados para el anuncio
* **Configuración de plataforma**: los campos de cuenta, campaña y configuración de otra plataforma utilizados para activar el anuncio

La vista de detalles de una activación fallida incluye el motivo del error.
