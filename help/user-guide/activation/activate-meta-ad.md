---
title: Activar un anuncio de Meta
description: Obtenga información sobre cómo activar una experiencia de anuncio de Meta.
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
TQID: https://experienceleague.adobe.com/hDR0ngNiGnCXCCOgNhVG8gX4kHGrNvfybPbuMLwYk7U
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
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
source-wordcount: '382'
ht-degree: 0%
---
# Activar un anuncio de Meta

Adobe GenStudio for Performance Marketing admite la activación de experiencias de anuncios de Meta en Instagram y Facebook.

**Formatos compatibles**: Imagen, Vídeo, Carrusel.

[Cree una experiencia Meta](/help/user-guide/create/create-meta-ad.md) en GenStudio for Performance Marketing y selecciónela para activarla.

La activación de un anuncio de Meta sigue los [mismos pasos generales](create-activation.md) necesarios para la activación en otros canales de publicidad pagada. Esta página cubre los requisitos previos específicos de Meta y los campos de configuración. Después de activar una experiencia de Meta en GenStudio for Performance Marketing, usa [Meta Ads Manager](https://adsmanager.facebook.com/) para revisar la experiencia e iniciar el anuncio.

A diferencia de otros canales, un anuncio de Meta puede incluir varias relaciones de aspecto dentro de un solo anuncio. Si su experiencia tiene múltiples relaciones de aspecto, [!DNL Activate] sigue generando solamente una fila para ella, no una fila por relación de aspecto.

Los administradores de sistemas y editores de GenStudio pueden activar las experiencias publicitarias.

## Requisitos previos

Confirme que las cuentas de publicidad de Meta conectadas tienen permiso total para administrar los anuncios de estos componentes de Meta Advertising Platform:

* Cuenta de Meta Ad
* Página de Facebook
* campaña de Meta
* Conjunto de anuncios de Meta
* Perfil de Instagram (opcional)

La campaña de Meta de destino y el conjunto de anuncios deben existir ya en el Administrador de Meta Ads. Actualmente, GenStudio for Performance Marketing no crea campañas ni conjuntos de anuncios.

## Conectar sus cuentas de Meta

Para que su organización pueda activar experiencias, un administrador del sistema de GenStudio debe conectar sus cuentas de Meta a GenStudio for Performance Marketing. Esta conexión permite que los datos fluyan entre GenStudio for Performance Marketing y Meta, lo que permite el proceso de activación. Ver [Conectarse a Meta Ads](/help/user-guide/connectors/meta-ads.md).

Para seleccionar una cuenta de Instagram, asegúrese en Meta Business Manager de que [la cuenta de Instagram que desea usar está conectada a la misma cuenta de publicidad](/help/user-guide/connectors/meta-ads.md#connect-an-instagram-account) seleccionada durante la incorporación. Si falta esta conexión, es posible que la cuenta de Instagram no aparezca en el menú desplegable **[!UICONTROL perfil de Instagram]** durante la activación.

Una vez finalizada la sincronización, puede ver las cuentas añadidas. Las grandes cantidades de datos tardan más en sincronizarse.

## Campos de configuración de Meta

Los recursos, titulares y copias de cuerpo aprobados están bloqueados y no se pueden editar durante la activación, puesto que ya se han revisado y aprobado en [!DNL Content]. Puede editar:

* **Campos de texto**: Descripción, Call-to-action, URL de destino, parámetros de URL, ID de seguimiento (se usa como nombre de anuncio de Meta)
* **Campos de configuración de plataforma**: Cuenta de publicidad, página de Facebook, perfil de Instagram, campaña de Meta, conjunto de anuncios de Meta
