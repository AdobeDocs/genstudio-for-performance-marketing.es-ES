---
title: Activar un anuncio de Innovid
description: Aprenda a activar una experiencia Innovid.
feature: Ad Activation
exl-id: ebb2aa9e-8efb-45b0-9ba2-7b27b8888708
TQID: https://experienceleague.adobe.com/VTzk2CDlTqawM1ckdHPVzs2ES-y0Ui0mkOLnVD88bJk
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%
---
# Activar un anuncio de Innovid

Adobe GenStudio for Performance Marketing admite la activación de experiencias publicitarias en Innovid.

**Formatos compatibles**: Pantalla estática, pantalla de código postal HTML5.

La activación de una experiencia Innovid sigue los [mismos pasos generales](create-activation.md) necesarios para la activación en otros canales de publicidad pagada. Esta página cubre los requisitos previos específicos de Innovid y los campos de configuración. Después de activar una experiencia en GenStudio for Performance Marketing, utilice Innovid para revisar la experiencia e iniciar el anuncio.

Los administradores de sistemas y editores de GenStudio pueden activar las experiencias publicitarias.

## Requisitos previos

* Acceso a la cuenta de destinatario Innovid.
* Acceso de administrador a esa cuenta, para leer y escribir en Innovid.

Innovid organiza campañas y anuncios dentro de diferentes cuentas, y cada cuenta tiene una biblioteca creativa. La biblioteca creativa de destino ya debe existir en Innovid; GenStudio for Performance Marketing publica experiencias de publicidad en esa biblioteca creativa, pero no crea cuentas ni bibliotecas creativas.

## Conecte su cuenta de Innovid

Para que su organización pueda publicar recursos en una biblioteca creativa, un administrador del sistema de GenStudio debe conectar su cuenta de Innovid a GenStudio for Performance Marketing. Debe tener acceso de administrador a esa cuenta para leer y escribir en Innovid. Ver [Conectar cuentas de medios pagados](/help/user-guide/connectors/connect-channel.md).

Una vez finalizada la sincronización, puede ver las cuentas añadidas.

## Campos de configuración Innovid

Los recursos aprobados están bloqueados y no se pueden editar durante la activación, puesto que ya se han revisado y aprobado en [!DNL Content]. Puede editar:

* **Campos de texto**: ID de seguimiento (usado como nombre creativo de la plataforma)
* **Campos de configuración de plataforma**: Cuenta, Biblioteca Creative, Nombre de concepto

La experiencia creativa se enviará a la biblioteca creativa seleccionada en Innovid cuando finalice la activación.
