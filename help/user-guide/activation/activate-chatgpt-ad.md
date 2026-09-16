---
title: Activar un anuncio de ChatGPT
description: Obtenga información sobre cómo activar una experiencia de publicidad de ChatGPT.
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
source-wordcount: '272'
ht-degree: 0%
---
# Activación de un anuncio de ChatGPT

Adobe GenStudio for Performance Marketing admite la activación de experiencias publicitarias de ChatGPT.

**Formatos compatibles**: Tarjetas de chat.

Puedes [crear una experiencia ChatGPT](/help/user-guide/create/create-chatgpt-ad.md) en GenStudio for Performance Marketing y luego seleccionarla para activarla.

La activación de un anuncio de ChatGPT sigue los [mismos pasos generales](create-activation.md) necesarios para la activación en otros canales de publicidad pagada. Esta página cubre los requisitos previos específicos de ChatGPT y los campos de configuración. Después de activar una experiencia ChatGPT en GenStudio for Performance Marketing, utilice OpenAI Ads Manager para ejecutar comprobaciones finales e iniciar el anuncio.

Los administradores de sistemas y editores de GenStudio pueden activar las experiencias publicitarias.

## Requisitos previos

* Una cuenta de OpenAI Ads y una clave de API de esa cuenta.
* La campaña de ChatGPT y el grupo de anuncios de destino ya deben existir en OpenAI Ads Manager. GenStudio for Performance Marketing no crea nuevas campañas ni grupos de anuncios.

## Conecte su cuenta de ChatGPT

Para que su organización pueda activar experiencias, un administrador del sistema de GenStudio debe conectar su cuenta de OpenAI Ads a GenStudio for Performance Marketing:

1. En el Administrador de anuncios de OpenAI, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Claves de API]** > **[!UICONTROL Crear nueva clave]**.
1. En GenStudio for Performance Marketing, ve a **[!UICONTROL Más]** > **[!UICONTROL Configuración]** > **[!UICONTROL ChatGPT]** > **[!UICONTROL Conectar]** > **[!UICONTROL Agregar cuenta]**.
1. Escriba el nombre de su cuenta de OpenAI Ads, pegue su clave de API y haga clic en **[!UICONTROL Agregar cuenta]**.

## Campos de configuración de ChatGPT

Los recursos aprobados, titulares (Título) y texto independiente están bloqueados y no se pueden editar durante la activación, puesto que ya se han revisado y aprobado en [!DNL Content]. Puede editar:

* **Campos de texto**: URL de destino, ID de seguimiento (usado como nombre de anuncio de plataforma)
* **Campos de configuración de plataforma**: Cuenta de OpenAI Ads, Campaña de OpenAI, grupo de anuncios de OpenAI

La dirección URL de destino debe utilizar un formato de `https://` válido, por ejemplo `https://www.example.com`.
