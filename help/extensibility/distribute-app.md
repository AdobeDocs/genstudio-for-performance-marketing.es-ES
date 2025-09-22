---
title: Distribuya su aplicación
description: Distribuya su aplicación, o complemento, para GenStudio for Performance Marketing.
feature: Extensibility
exl-id: 4935356b-08df-402c-b1a2-b89627afc188
source-git-commit: 6ba402e9cdfb62d71c9993457a6d9952c4877553
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Distribuya su aplicación

La distribución del complemento lo hace disponible para su uso por parte de su organización y otras personas.El flujo de trabajo de distribución depende de si el complemento está pensado para su distribución pública o privada.

En este tema se describe la distribución privada. La distribución privada restringe la implementación del complemento a la organización, identificada por la organización de IMS, para la que se desarrolló.

La distribución pública hace que el complemento esté disponible como aplicación en Adobe Exchange. [Distribución pública](https://developer.adobe.com/app-builder/docs/guides/distribution/public/) en la documentación para desarrolladores de _App Builder_ describe cómo poner tu aplicación a disposición de cualquier organización de Adobe.

>[!BEGINSHADEBOX]

**Requisitos previos**:

Confirme los siguientes permisos:

* Permisos de desarrollador en la organización desde la que envía la aplicación para su aprobación

* Permisos del administrador del sistema para aprobar la aplicación

La aplicación de App Builder debe implementarse en un proyecto de App Builder.

>[!ENDSHADEBOX]

**Para distribuir la aplicación de forma privada**:

La distribución privada hace que la aplicación solo esté disponible para los miembros de la organización.

1. En [Adobe Developer Console](https://developer.adobe.com/console/), seleccione la organización, el proyecto y el espacio de trabajo donde se implementa la aplicación.

1. Seleccione [!UICONTROL Aprobación] en el área de _Información general de Workspace_. Se abre el panel _Aprobación de aplicación_.

1. En el área _Detalles de envíos de aplicaciones_, agregue detalles informativos sobre su complemento. Los detalles incluyen nombre de la aplicación, descripción y correo electrónico de contacto.

1. Cuando haya completado todos los campos, haga clic en [!UICONTROL Enviar].

1. Inicie sesión en [Adobe Exchange](https://exchange.adobe.com/) con el mismo Adobe ID que utilizó para iniciar sesión en Developer Console. Si no tiene permisos de administrador del sistema en esta organización, solicite la aprobación a un administrador del sistema de la organización.

1. Seleccione [!UICONTROL Administrar] > [!UICONTROL aplicaciones de App Builder] para acceder a una solicitud y revisar la aplicación.

1. Después de revisar la aplicación, selecciona [!UICONTROL Aprobar]. También puede agregar notas informativas.

El complemento ahora está visible en la instancia de GenStudio for Performance Marketing de su organización.
