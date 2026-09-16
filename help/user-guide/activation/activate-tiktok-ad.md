---
title: Activar un anuncio de TikTok
description: Obtenga información sobre cómo activar una experiencia de anuncio de vídeo en fuente de TikTok.
feature: Ad Activation
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
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%
---
# Activar un anuncio de TikTok

Adobe GenStudio for Performance Marketing admite la activación de experiencias de anuncios de TikTok.

**Formatos compatibles**: Anuncios de vídeo en la fuente.

Puedes [crear una experiencia de TikTok](/help/user-guide/create/tiktok-experiences.md) en GenStudio for Performance Marketing y luego seleccionarla para activarla.

La activación de un anuncio de TikTok sigue los [mismos pasos generales](create-activation.md) necesarios para la activación en otros canales de publicidad pagada. Esta página cubre los requisitos previos específicos de TikTok y los campos de configuración. Después de activar una experiencia de TikTok en GenStudio for Performance Marketing, utilice el Administrador de TikTok Ads para ejecutar las comprobaciones finales e iniciar el anuncio.

Los administradores de sistemas y editores de GenStudio pueden activar las experiencias publicitarias.

## Requisitos previos

* Una cuenta de TikTok Ads con acceso de operador o administrador.
* Al menos una cuenta de publicidad de TikTok habilitada para su uso y conectada a un administrador del sistema o editor de GenStudio.
* La campaña de TikTok de destino ya debe existir en el Administrador de TikTok Ads. TikTok Ads Manager, no GenStudio for Performance Marketing, define el presupuesto, la oferta, la optimización y el objetivo del grupo de publicidad.

## Conecte su cuenta de TikTok

Para que su organización pueda activar experiencias, un administrador del sistema de GenStudio debe conectar su cuenta de TikTok Ads a GenStudio for Performance Marketing:

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL TikTok]** > **[!UICONTROL Conectar]**.
1. Inicie sesión en la cuenta de TikTok Ads Manager en la ventana que se abre y complete el inicio de sesión de OAuth. Su cuenta debe tener acceso de operador o administrador a la cuenta publicitaria.

Una vez finalizada la conexión, confirme que hay al menos una cuenta de publicidad de TikTok habilitada para su uso.

## Campos de configuración de TikTok

Los recursos aprobados y el texto principal están bloqueados y no se pueden editar durante la activación, puesto que ya se han revisado y aprobado en [!DNL Content]. Puede editar:

* **Campos de texto**: Call-to-action, URL de destino, ID de seguimiento (usado como nombre de anuncio de plataforma)
* **Campos de configuración de plataforma**: Cuenta de TikTok Ads, Campaña, Grupo de anuncios
