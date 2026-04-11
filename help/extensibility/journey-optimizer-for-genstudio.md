---
title: Journey Optimizer para GenStudio
description: Instale y configure la aplicación de Journey Optimizer para GenStudio Adobe Exchange para que su organización pueda utilizar plantillas de Adobe Journey Optimizer en GenStudio for Performance Marketing.
feature: Extensibility
source-git-commit: fbec4567d960a6e3607c5e5e43057e2f22e9f6ea
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# Journey Optimizer para GenStudio

Las organizaciones que usan [!DNL Adobe Journey Optimizer] (AJO) y [!DNL GenStudio for Performance Marketing] en la misma organización [!DNL IMS] pueden instalar la aplicación **Journey Optimizer for GenStudio** desde [!DNL Adobe Exchange]. Una vez que un administrador del sistema aprueba la aplicación y completa la implementación, los autores pueden elegir plantillas de contenido de AJO al crear experiencias de correo electrónico en GenStudio, junto a las plantillas cargadas directamente en [!DNL Content].

Este tema es para **administradores y desarrolladores** que instalan la aplicación, crean credenciales de OAuth en [!DNL Adobe Developer Console] y asignan permisos de cuenta técnica en [!DNL Adobe Experience Platform]. Para saber cómo funciona la sintaxis de plantillas de AJO y Marketo con GenStudio, consulte [Plantillas de AJO y Marketo](/help/user-guide/templates/use-templates.md#templates-from-ajo-and-marketo).

## Requisitos previos

* AJO debe estar aprovisionado en la organización en la que implementa la extensión.
* Los usuarios que crean plantillas en AJO necesitan permiso para **crear y editar** plantillas de contenido en Journey Optimizer, tal como lo define su organización.
* Las plantillas de correo electrónico de AJO deben incluir marcadores de posición de campo (controladores) en los que debe aparecer el contenido generado. Se puede seleccionar una plantilla sin esos campos, pero **la generación de la experiencia falla** si faltan los marcadores de posición [!DNL GenStudio for Performance Marketing] esperados. Ver [Personalizar una plantilla](/help/user-guide/templates/customize-template.md) y [nombres de campo reconocidos](/help/user-guide/templates/customize-template.md#recognized-field-names).

## Instalación de la aplicación desde Adobe Exchange

>[!VIDEO](https://video.tv.adobe.com/v/3483302?captions=spa&learn=on)

1. Abra [Adobe Exchange](https://exchange.adobe.com) y vaya a **[!UICONTROL Experience Cloud]**.
1. Abra el listado de [Journey Optimizer for GenStudio](https://exchange.adobe.com/apps/ec/abpopqqr1q/journey-optimizer-for-genstudio).
   ![Anuncio de Journey Optimizer for GenStudio en Adobe Exchange, incluidos requisitos e instalación gratuita](/help/extensibility/ajo-adobe-exchange.png){width="75%"}
1. Seleccione **[!UICONTROL Gratis]** para solicitar la aplicación para su organización.
1. Una vez que su organización **revise y apruebe** la solicitud, continúe con [Crear credenciales de OAuth en Adobe Developer Console](#create-oauth-credentials-in-adobe-developer-console) e [Implemente la aplicación desde Exchange](#deploy-the-application-from-exchange).

## Crear credenciales de OAuth en Adobe Developer Console

Cree un **proyecto** en [Adobe Developer Console](https://developer.adobe.com/console/) que proporcione credenciales de OAuth para la API de Journey Optimizer. Necesitará valores como **ID de cliente**, **Secreto de cliente**, **ID de organización** y **Ámbito** al configurar la aplicación en Exchange.

1. Inicie sesión en Adobe Developer Console y cree un **nuevo proyecto**.
1. Agregue la API **Adobe Journey Optimizer (AJO)** al proyecto haciendo clic en **[!UICONTROL Agregar API]** y seleccionando **[!UICONTROL Adobe Journey Optimizer]** de la lista de API de producto **[!DNL Experience Cloud]**.
1. Genere credenciales en el área de trabajo del proyecto y copie **ID de cliente**, **Secreto de cliente**, **ID de organización**, **Ámbito** y cualquier otro valor que solicite su flujo de implementación. Guárdelos de forma segura en la siguiente sección.

>[!NOTE]
>
>Cuando realice la instalación desde Exchange, utilice el **ID de cliente de OAuth** si se muestran tanto un ID de cliente de OAuth como un ID de cuenta técnica.

## Implementar la aplicación desde Exchange

### Abra la aplicación en Administrar y añada un entorno

1. Volver a [Adobe Exchange](https://exchange.adobe.com).
1. Seleccione **[!UICONTROL Administrar]** y abra **[!UICONTROL aplicaciones de App Builder]** (o la ruta de su organización a las aplicaciones administradas).
1. Seleccione **Journey Optimizer para GenStudio** y confirme que la aplicación está **aprobada**.
1. En **[!UICONTROL Entornos]**, elija un entorno existente del menú desplegable **Entornos:** o seleccione **[!UICONTROL Agregar entorno]** para crear uno.
   ![Detalles de la aplicación con estado Aprobado y Agregar entorno](/help/extensibility/ajo-config-002.png){width="50%"}
1. En el entorno seleccionado, seleccione **[!UICONTROL Configuración]**.
1. En la ficha **[!UICONTROL Configuración]**, busque **[!UICONTROL Credenciales de AJO]**.
   ![Configuración con credenciales de AJO antes de la implementación (borrador)](/help/extensibility/ajo-config-004.png){width="80%"}
1. Introduzca las credenciales del proyecto de Developer Console que tiene la API de Journey Optimizer agregada (por ejemplo, **[!UICONTROL ID de cliente de AJO]**, **[!UICONTROL Secreto de cliente de AJO]**, y **[!UICONTROL Extremo de token de AJO]** y cualquier otro campo obligatorio).
1. Escriba el nombre de la zona protegida **en minúsculas** (por ejemplo, `prod`).
1. Haga clic en **[!UICONTROL Implementar]**. Cuando finaliza la implementación, el estado se muestra como implementado. El texto del botón cambiará a **[!UICONTROL Anular implementación]**.
   ![Aplicación implementada con anulación de implementación disponible en la vista de aplicaciones de App Builder](/help/extensibility/ajo-config-005.png){width="80%"}

Después de la implementación, Adobe Developer Console incluye un nuevo proyecto generado automáticamente denominado **Journey Optimizer for GenStudio &lt;Your_Environment_Name>** con las API de AJO y Adobe Runtime. Este proyecto es de solo lectura y no se puede editar ni eliminar.
![Proyecto de Developer Console de solo lectura generado automáticamente después de la implementación](/help/extensibility/ajo-auto-project.png){width="100%"}

### Actualizar configuración

Para cambiar las variables de configuración de un entorno, **[!UICONTROL Anular la implementación]** primero, actualice los valores y, a continuación, **[!UICONTROL Implementar]** de nuevo para que los cambios surtan efecto.

Puede crear **varios entornos** en Exchange (por ejemplo, uno por zona protegida). Cada implementación puede aparecer como una experiencia independiente en GenStudio cuando su organización utiliza varias zonas protegidas.

## Asignación de permisos para la cuenta técnica

Los usuarios pueden ver la extensión de AJO en GenStudio sin acceso completo de [!DNL Adobe Experience Platform]. Para las llamadas API (por ejemplo, cargar plantillas), la cuenta técnica vinculada a las credenciales de OAuth debe tener permisos de Journey Optimizer en **[!DNL Adobe Experience Platform]** > **[!UICONTROL Permisos]**. Los nombres de funciones y conjuntos de permisos exactos dependen de su organización.

Vea la extensión en **[!UICONTROL Administrador de Recorrido]** en AJO **[!UICONTROL Permisos]** > **[!UICONTROL Roles]** y agregue las **credenciales de API** desde el proyecto de Developer Console, las mismas credenciales que utilizó al implementar desde Exchange.

![Credenciales de API asignadas a la función de arquitecto de AJO en Permisos de Adobe Experience Platform](/help/extensibility/ajo-map-permissions.png){width="80%"}

**Ver también** (control de acceso de Journey Optimizer):

* [Control de acceso](https://experienceleague.adobe.com/es/docs/journey-optimizer/using/access-control/access-control-landing-page)
* [Permisos en Journey Optimizer](https://experienceleague.adobe.com/es/docs/journey-optimizer/using/access-control/permissions)
* [Introducción para administradores de sistemas](https://experienceleague.adobe.com/es/docs/journey-optimizer/using/get-started/quick-start/administrator)

## Acceso a plantillas de AJO en GenStudio

Después de la implementación y asignación de permisos:
1. Abra **[!UICONTROL Crear]** en GenStudio for Performance Marketing e inicie una experiencia de **correo electrónico**.
1. En **[!UICONTROL Seleccionar plantilla]**, abra la ficha **[!UICONTROL Plantilla de AJO]** junto a **[!UICONTROL Plantillas cargadas]** para examinar las plantillas de Journey Optimizer.

![Seleccionar plantilla con la ficha Plantilla de AJO y la galería de plantillas](/help/extensibility/ajo-template-tab.png){width="80%"}

## Resolución de problemas

### La pestaña Plantillas de AJO no está visible

* Confirme que los valores especificados en Exchange **[!UICONTROL Configuration]** son correctos, incluidos **ID de cliente**, **Secreto de cliente**, **Ámbito** y **espacio aislado**.
* Asegúrese de que el nombre de la zona protegida **esté en minúsculas** (por ejemplo, `prod`).
* Al instalar desde Exchange, use el **ID de cliente** como se describe en [Crear credenciales de OAuth](#create-oauth-credentials-in-adobe-developer-console).

### La pestaña Plantillas de AJO está visible, pero no aparece ninguna

* Vuelva a cargar la página o abra la ficha **[!UICONTROL Plantilla de AJO]**.
* En las herramientas del explorador **[!UICONTROL Red]**, inspeccione la solicitud **`get-templates`**. Si devuelve **403 Prohibido**, la cuenta técnica no se asigna a un rol o grupo con los permisos de Journey Optimizer necesarios. Actualice las asignaciones en [!DNL Adobe Experience Platform] **[!UICONTROL Permisos]** y en AJO **[!UICONTROL Permisos]** según lo requiera su organización.
