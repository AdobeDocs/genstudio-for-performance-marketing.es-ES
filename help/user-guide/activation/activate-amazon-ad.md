---
title: Activar Amazon Ads
description: Obtenga información sobre cómo activar experiencias de Amazon Ads.
feature: Ad Activation
exl-id: 539cb43c-a9d8-4473-8a7d-e81967111741
TQID: https://experienceleague.adobe.com/4L4JHcYLSsoQ50QbCW7Mof52h5jpz3z8n0UL8CaqLA8
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
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%
---
# Activar Amazon Ads

Adobe GenStudio for Performance Marketing admite la activación de experiencias publicitarias en Amazon Ads.

**Formatos compatibles**: Visualización estática.

La activación de una experiencia de Amazon Ads sigue los [mismos pasos generales](create-activation.md) necesarios para la activación en otros canales de anuncios pagados. Esta página cubre los requisitos previos y los campos de configuración específicos de Amazon Ads. Después de activar una experiencia en GenStudio for Performance Marketing, utilice Amazon Ads para revisar la experiencia e iniciar el anuncio.

Los administradores de sistemas y editores de GenStudio pueden activar las experiencias publicitarias.

## Requisitos previos

* Acceso a la cuenta de Amazon Ads de destinatario.
* Acceso de administrador a esa cuenta para leer y escribir en Amazon Ads.

Amazon Ads organiza campañas y anuncios en cuentas diferentes, y cada cuenta incluye una biblioteca creativa. La cuenta de destino ya debe existir en Amazon Ads; GenStudio for Performance Marketing publica experiencias de publicidad en la biblioteca creativa de esa cuenta, pero no crea cuentas.

## Conecte su cuenta de Amazon Ads

Para que su organización pueda publicar recursos en una biblioteca creativa, un administrador del sistema de GenStudio debe conectar su cuenta de Amazon Ads a GenStudio for Performance Marketing. Debe tener acceso de administrador a esa cuenta para leer y escribir en Amazon Ads. Ver [Conectar cuentas de medios pagados](/help/user-guide/connectors/connect-channel.md).

Una vez finalizada la sincronización, puede ver las cuentas añadidas.

## Campos de configuración de Amazon Ads

Los recursos aprobados están bloqueados y no se pueden editar durante la activación, puesto que ya se han revisado y aprobado en [!DNL Content]. Puede editar:

* **Campos de texto**: ID de seguimiento (usado como nombre creativo de la plataforma)
* **Campos de configuración de plataforma**: Cuenta

La experiencia creativa se enviará a la biblioteca creativa de la cuenta seleccionada en Amazon Ads cuando finalice la activación.
