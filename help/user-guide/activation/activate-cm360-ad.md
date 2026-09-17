---
title: Activación de un anuncio de Google Campaign Manager 360
description: Obtenga información sobre cómo activar una experiencia de Google Campaign Manager 360.
feature: Ad Activation
exl-id: e4ee4e04-8dd0-4e05-a0f7-0ddca2fbb6be
TQID: https://experienceleague.adobe.com/pQbT2OC7-jK33HhJWgTBBtJrmEvr48mGkl8v-fTkOLQ
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%
---
# Activar un anuncio de Google Campaign Manager 360

Adobe GenStudio for Performance Marketing admite la activación de experiencias publicitarias en Google Campaign Manager 360.

**Formatos compatibles**: Pantalla estática, Pantalla de vídeo, Pantalla con código postal HTML5.

La activación de un anuncio de Google Campaign Manager 360 sigue los [mismos pasos generales](create-activation.md) necesarios para la activación en otros canales de publicidad pagada. Esta página cubre los requisitos previos y los campos de configuración específicos de Google Campaign Manager 360. Después de activar una experiencia en GenStudio for Performance Marketing, utilice Google Campaign Manager 360 para revisar la experiencia e iniciar el anuncio.

Los administradores de sistemas y editores de GenStudio pueden activar las experiencias publicitarias.

## Requisitos previos

* Una cuenta de Google Campaign Manager 360 con acceso al anunciante de destinatario.
* Acceso de administrador al anunciante para leer y escribir en Campaign Manager 360.

Campaign Manager 360 organiza campañas y anuncios en diferentes anunciantes, y cada anunciante incluye una biblioteca creativa. El anunciante de destino ya debe existir en Campaign Manager 360; GenStudio for Performance Marketing publica experiencias de publicidad en la biblioteca creativa de ese anunciante, pero no crea anuncios.

## Conecte su cuenta de Google Campaign Manager 360

Para que su organización pueda publicar recursos en una biblioteca creativa, un administrador del sistema o editor de GenStudio debe conectar su cuenta de Google Campaign Manager 360 a GenStudio for Performance Marketing. Debe tener acceso de administrador al anunciante para leer y escribir en Campaign Manager 360. Ver [Conectar cuentas de medios pagados](/help/user-guide/connectors/connect-channel.md).

Una vez finalizada la sincronización, puede ver las cuentas añadidas.

## Campos de configuración de Google Campaign Manager 360

Los recursos aprobados están bloqueados y no se pueden editar durante la activación, puesto que ya se han revisado y aprobado en [!DNL Content]. Puede editar:

* **Campos de texto**: ID de seguimiento (usado como nombre creativo de la plataforma)
* **Campos de configuración de plataforma**: Anunciante

La experiencia creativa se envía a la biblioteca creativa del anunciante seleccionado en Google Campaign Manager 360 cuando se completa la activación.
