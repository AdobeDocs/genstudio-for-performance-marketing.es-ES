---
title: Activación de un anuncio de LinkedIn
description: Obtenga información sobre cómo activar una experiencia de publicidad de LinkedIn.
feature: Ad Activation
exl-id: edc95319-36c3-4cbf-a5c0-865b49482b50
TQID: https://experienceleague.adobe.com/1mcxWePqYd8tYp3e1D2UTSeBHSvPj4WrqeSyiUCxD8c
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
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%
---
# Activación de un anuncio de LinkedIn

Adobe GenStudio for Performance Marketing admite la activación de experiencias de anuncios de LinkedIn en [Administrador de campañas de LinkedIn](https://business.linkedin.com/marketing-solutions).

**Formatos compatibles**: Imagen única, Vídeo único.

Puede [crear una experiencia de LinkedIn](/help/user-guide/create/create-linkedin.md) en GenStudio for Performance Marketing y luego seleccionarla para su activación.

La activación de un anuncio de LinkedIn sigue los [mismos pasos generales](create-activation.md) necesarios para la activación en otros canales de publicidad pagada. Esta página cubre los requisitos previos específicos de LinkedIn y los campos de configuración. Después de activar una experiencia de LinkedIn en GenStudio for Performance Marketing, utilice el administrador de LinkedIn Campaign para revisar la experiencia e iniciar el anuncio.

Los administradores de sistemas y editores de GenStudio pueden activar las experiencias publicitarias.

## Requisitos previos

* Una cuenta de LinkedIn Campaign Manager con permiso total para administrar campañas y anuncios. Esta cuenta debe contener campañas existentes.
* Cuentas de anuncios de LinkedIn con permiso total para crear anuncios y publicar contenido en páginas de LinkedIn.

La campaña de LinkedIn de destino y el conjunto de anuncios ya deben existir en el Administrador de campañas de LinkedIn. GenStudio for Performance Marketing no crea campañas ni conjuntos de anuncios.

>[!NOTE]
>
>LinkedIn cambió el nombre de su jerarquía de campañas: lo que LinkedIn Campaign Manager llamaba anteriormente **grupo de campañas** ahora se llama **campaña**, y lo que antes llamaba **campaña** ahora se llama **conjunto de anuncios**. Los campos de configuración **[!UICONTROL LinkedIn campaign]** y **[!UICONTROL LinkedIn ad set]** en [!DNL Activate] utilizan esta terminología actual.

Actualmente, GenStudio for Performance Marketing admite anuncios LinkedIn de una sola imagen y un solo vídeo, y cada uno de ellos lleva una sola imagen o vídeo por publicación. Si la experiencia incluye varias proporciones de aspecto, [!DNL Activate] genera una fila por proporción independiente en la tabla de activación para que cada una pueda ejecutarse como su propia publicidad; elimine las filas que no necesite.

## Conectar sus cuentas de LinkedIn

Para que su organización pueda activar experiencias, un administrador del sistema o un editor de GenStudio deben conectar sus cuentas de publicidad de LinkedIn a GenStudio for Performance Marketing. Debe tener acceso de administrador completo a la cuenta de publicidad y a la página de perfil de LinkedIn para conectarse correctamente. Solo tiene que conectar una cuenta de publicidad en **[!UICONTROL Configuración]** una vez. Después de eso, está disponible para cualquier persona que pueda acceder a esa instancia.

Esta conexión permite que los datos fluyan entre GenStudio for Performance Marketing y LinkedIn, lo que permite el proceso de activación.

Una vez finalizada la sincronización, puede ver las cuentas añadidas. Las grandes cantidades de datos tardan más en sincronizarse.

## Campos de configuración de LinkedIn

Los recursos, titulares y texto introductorio aprobados están bloqueados y no se pueden editar durante la activación, puesto que ya se han revisado y aprobado en [!DNL Content]. Puede editar:

* **Campos de texto**: Descripción, Call-to-action, URL de destino, parámetros de URL, ID de seguimiento (se usa como nombre de anuncio de plataforma)
* **Campos de configuración de plataforma**: Cuenta de publicidad de LinkedIn, campaña de LinkedIn, conjunto de anuncios de LinkedIn
