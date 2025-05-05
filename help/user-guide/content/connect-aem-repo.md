---
title: Conectar con un  [!DNL AEM Assets Content Hub] repositorio
description: Aprenda a conectar Adobe GenStudio for Performance Marketing a un repositorio de Adobe Experience Manager (AEM) [!DNL Content Hub] y a aprovechar el contenido aprobado existente.
level: Experienced
role: Admin, Data Engineer
feature: Content Management
recommendations: noDisplay
exl-id: abb587fd-593c-4b9f-baad-993d92400d9b
source-git-commit: 85948ccd9b6d198a2064d95639f96a045ea61743
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Conectar a un repositorio [!DNL AEM Assets Content Hub]

Si tiene recursos en Adobe Experience Manager (AEM), puede seguir estos pasos para que sean accesibles en GenStudio for Performance Marketing.

>[!BEGINSHADEBOX]

**Requisitos previos**:

Los siguientes pasos requieren acceso administrativo a Admin Console y a AEM Assets as a Cloud Service.

>[!ENDSHADEBOX]

## Paso 1: Habilitar [!DNL AEM Assets Content Hub]

Siga el proceso de autoservicio **Implementar Content Hub** para habilitar [!DNL Content Hub] para los AEM Assets existentes en Cloud Manager. Ver [Implementar [!DNL Content Hub]](https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub) en la documentación de _AEM as a Cloud Service_.

Después de habilitar [!DNL AEM Assets Content Hub], tiene una nueva instancia con el sufijo `contenthub` en [!DNL AEM Assets as a Cloud Service] en Admin Console.

>[!IMPORTANT]
>
>Los administradores deben comprobar que el repositorio [!DNL AEM Assets Content Hub] se encuentra en la misma organización que GenStudio for Performance Marketing.

## Paso 2: Incorporar usuarios de GenStudio

En [!DNL Admin Console], agregue un usuario o grupo de usuarios de GenStudio for Performance Marketing al perfil de producto [!DNL AEM Assets Content Hub]. Si un revisor de contenido no tiene acceso a la misma organización que el repositorio [!DNL AEM Assets Content Hub], puede que tenga dificultades para revisar y aprobar el contenido.

- [Incorporado [!DNL Content Hub] administrador](https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-administrator)
- [Incorporar [!DNL Content Hub] usuarios](https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-users)

## Paso 3: Aprobar los recursos

Apruebe los recursos para usarlos en [!DNL AEM Assets Content Hub], lo cual los hace disponibles en GenStudio for Performance Marketing.

Consulte [Aprobar recursos en Experience Manager](https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/approve-assets) en la documentación de _AEM as a Cloud Service_.

## Paso 4: Configurar la visibilidad de los recursos

En las opciones de configuración de _[!DNL AEM Assets Content Hub]_, revise cada conjunto de opciones de configuración para ver los filtros, los detalles de recursos, la búsqueda y la personalización de marca.

Consulte [Configuración de la interfaz de usuario de Content Hub](https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/content-hub/configure-content-hub-ui-options) en la documentación de _AEM as a Cloud Service_.

## Paso 5: Verificar la conexión

En el contenido de GenStudio for Performance Marketing, la lista _[!UICONTROL Ubicación]_ está disponible encima de la galería, en el lado derecho. La lista no está disponible si no tiene acceso o si su organización no ha implementado y conectado un repositorio [!DNL AEM Assets Content Hub].

Consulte [Ubicación de Assets](manage-assets.md#assets-location) para obtener información sobre la lista Ubicación y los repositorios que se están cambiando.
