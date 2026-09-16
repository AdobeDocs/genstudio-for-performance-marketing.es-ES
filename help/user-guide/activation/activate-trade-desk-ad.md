---
title: Activación de un anuncio en Trade Desk
description: Aprenda a activar una experiencia de anuncio de visualización estática en Trade Desk.
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
source-wordcount: '461'
ht-degree: 0%
---
# Activación de un anuncio en Trade Desk

Adobe GenStudio for Performance Marketing admite la activación de experiencias publicitarias en Trade Desk.

**Formatos admitidos**: Visualización estática (solo de un recurso).

La activación de un anuncio en Trade Desk sigue los [mismos pasos generales](create-activation.md) necesarios para la activación en otros canales de publicidad de pago, con una diferencia. Trade Desk es un servicio empresarial administrado, no una plataforma de anuncios de autoservicio, por lo que el acceso a la cuenta funciona de forma diferente que para otros canales. Esta página cubre esas diferencias junto con los requisitos previos y los campos de configuración específicos de la Oficina de Comercio.

Los administradores de sistemas y editores de GenStudio pueden activar las experiencias publicitarias.

## Requisitos previos

* Una cuenta existente de la Oficina de Comercio en directo. Configúrelo directamente con la Oficina de Comercio antes de conectarlo a GenStudio for Performance Marketing.
* Acceso a la API habilitado por el equipo de cuenta de The Trade Desk. Para Trade Desk, su equipo de cuenta habilita este acceso en su nombre mediante un token de API, en lugar del inicio de sesión de OAuth utilizado por otros canales de publicidad pagada.
* El anunciante, el puesto y los permisos correctos que ha habilitado Trade Desk para la integración de GenStudio for Performance Marketing.
* Un token de API o credenciales de su equipo de cuenta de The Trade Desk, con permisos para publicar creativos en la cuenta del anunciante de destinatario.
* Una campaña de destino que ya existe en Trade Desk. GenStudio for Performance Marketing activa los anuncios en esa campaña existente.

## Conecte su cuenta de The Trade Desk

Antes de que su organización pueda activar experiencias, trabaje con su equipo de cuenta de The Trade Desk para habilitar el acceso a la API y, a continuación, un administrador del sistema de GenStudio conectará la cuenta a GenStudio for Performance Marketing:

1. Póngase en contacto con el equipo de cuenta de The Trade Desk y solicite acceso para publicar elementos creativos de GenStudio for Performance Marketing en su cuenta de The Trade Desk. Confirme el ID del anunciante, el puesto o los detalles del socio que se utilizarán para la activación.
1. Obtenga el token de API o las credenciales de su equipo de cuenta de The Trade Desk y confirme que el token admite permisos de publicación creativa para la cuenta del anunciante de destino.
1. En GenStudio for Performance Marketing, ve a **[!UICONTROL Configuración]** > **[!UICONTROL Canales]** y, a continuación, haz clic en **[!UICONTROL Conectar]** en el mosaico **[!UICONTROL The Trade Desk]**. Introduzca el nombre de la cuenta, el ID del anunciante y el token o las credenciales de la API. A continuación, guarde la conexión.

Si la conexión falla, confirme con el equipo de cuenta de The Trade Desk que el acceso a la API se ha habilitado y que el token tiene el anunciante y los permisos de asiento correctos.

## Los campos de configuración de la Trade Desk

Los recursos aprobados están bloqueados y no se pueden editar durante la activación, puesto que ya se han revisado y aprobado en [!DNL Content]. Puede editar:

* **Campos de texto**: ID de seguimiento (usado como nombre creativo de la plataforma)
* **Campos de configuración de plataforma**: Cuenta, Campaña

En este momento, la activación en The Trade Desk solo admite anuncios estáticos de visualización de un solo recurso.
