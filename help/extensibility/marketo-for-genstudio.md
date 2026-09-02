---
title: Marketo para GenStudio
description: Instale y configure la aplicación de Marketo para GenStudio Adobe Exchange para que su organización pueda utilizar plantillas de Marketo Engage en GenStudio for Performance Marketing.
feature: Extensibility
source-git-commit: e5011c95e9536d73b1f09d6bc76bb83f121573cd
workflow-type: tm+mt
source-wordcount: '955'
ht-degree: 0%

---

# Marketo para GenStudio

Las organizaciones que usan [!DNL Marketo Engage] y [!DNL GenStudio for Performance Marketing] en la misma organización de [!DNL IMS] pueden instalar la aplicación **Marketo for GenStudio** desde [!DNL Adobe Exchange]. Una vez que un administrador del sistema aprueba la aplicación y completa la implementación, los autores pueden elegir plantillas de Marketo al crear experiencias de correo electrónico en GenStudio, junto a las plantillas cargadas directamente en [!DNL Content].

Este tema es para **administradores** que instalan la aplicación, recopilan credenciales de Marketo e implementan la aplicación en Exchange. Para saber cómo funciona la sintaxis de plantillas de AJO y Marketo con GenStudio, consulte [Plantillas de AJO y Marketo](/help/user-guide/templates/use-templates.md#templates-from-ajo-and-marketo).

## Requisitos previos

* [!DNL Marketo Engage] debe estar aprovisionado en la organización en la que implementa la extensión.
* Los usuarios que implementan la aplicación necesitan **credenciales de Marketo**. Para crear y recuperar esas credenciales, debe tener acceso de **Administrador de productos de Marketo** (el área de **[!UICONTROL Administrador]** debe estar disponible cuando abra Marketo).

## Instalación de la aplicación desde Adobe Exchange

>[!VIDEO](https://video.tv.adobe.com/v/3483314?captions=spa&learn=on)

1. Abra [Adobe Exchange](https://exchange.adobe.com) y vaya a **[!UICONTROL CX Enterprise]**.
1. Abra el listado de [Marketo for GenStudio](https://exchange.adobe.com/apps/ec/ab6p21vo8r/marketo-for-genstudio).
   ![Listado de Marketo for GenStudio en Adobe Exchange](/help/extensibility/marketo-adobe-exchange.png){width="75%"}
1. Seleccione **[!UICONTROL Gratis]** para solicitar la aplicación para su organización.
1. Una vez que su organización **revise y apruebe** la solicitud, continúe con [Obtener credenciales de Marketo](#get-marketo-credentials) e [Implemente la aplicación desde Exchange](#deploy-the-application-from-exchange).

## Obtener credenciales de Marketo

Utiliza las credenciales de tu instancia de **Marketo** (no la Adobe Developer Console). Recopile las siguientes credenciales siguiendo los pasos que se indican a continuación antes de implementar en Exchange.

>[!NOTE]
>
>Para generar y recuperar las credenciales de Marketo, debe tener acceso de administrador de productos de Marketo; de lo contrario, la pestaña Administración no estará visible en Marketo.

### Crear un usuario solo de API (opcional si vuelve a utilizar un usuario de API existente)

1. En Marketo, ve a **[!UICONTROL Admin]**.
   ![Ficha de administración de Marketo](/help/extensibility/marketo-admin-global.png){width="80%"}
1. En **[!UICONTROL Seguridad]**, abra **[!UICONTROL Usuarios y roles]** y vaya a la ficha **[!UICONTROL Roles]**.
1. Cree una nueva función o edite una función existente, con los siguientes permisos agregados: _Access API_ y _Access Design Studio_.
1. Para un nuevo usuario de API, haga clic en **[!UICONTROL Crear usuario solo de API]** (use un correo electrónico único para cada usuario de API).
1. Seleccione la casilla de verificación de Roles y asigne el nuevo rol que ha creado. Si ya tiene un usuario de API que desee usar, vaya a [Crear o seleccionar un servicio de LaunchPoint](#create-or-select-a-launchpoint-service).

![Usuarios y funciones con funciones de API y usuario solo de API](/help/extensibility/marketo-users-roles-api-user.png){width="80%"}

### Crear o seleccionar un servicio de LaunchPoint

1. En **[!UICONTROL Admin]**, en **[!UICONTROL Integration]**, abra **[!UICONTROL LaunchPoint]**.
1. Haga clic en **[!UICONTROL Crear]** para crear un nuevo servicio (o use un servicio personalizado existente).
   ![Servicio personalizado de LaunchPoint](/help/extensibility/marketo-launchpoint-custom-service.png){width="80%"}
1. Para tu servicio, haz clic en **[!UICONTROL Ver detalles]** y copia el **[!UICONTROL ID de cliente]** y el **[!UICONTROL Secreto de cliente]**. Los introducirá en Adobe Exchange **[!UICONTROL Configuration]**.

### Anote la URL base de la API de REST de Marketo

1. En **[!UICONTROL Administrador]**, en **[!UICONTROL Integración]**, abra **[!UICONTROL Servicios web]**.
1. Busque el extremo **[!UICONTROL API de REST]**. Copie solamente la **dirección URL base** (host) con el formato `https://###-XXX-###.mktorest.com`. **no** incluye segmentos de ruta como `/rest` o `/identity`. Este valor es único para cada instancia de Marketo.

![URL base de extremo de API de REST de servicios web](/help/extensibility/marketo-web-services-rest-endpoint.png){width="80%"}

También necesitará la **[!UICONTROL URL de identidad de Marketo Engage]** que solicita la pantalla de implementación de Exchange, junto con la URL base de REST, el ID de cliente y el secreto de cliente de LaunchPoint.

## Implementar la aplicación desde Exchange

Para que la extensión esté disponible en GenStudio, implemente la aplicación desde Adobe Exchange.

1. Volver a [Adobe Exchange](https://exchange.adobe.com).
1. Seleccione **[!UICONTROL Administrar]** y abra la aplicación **Marketo for GenStudio** (por ejemplo, en **[!UICONTROL aplicaciones de App Builder]** o en las aplicaciones administradas de su organización).
1. En **[!UICONTROL Entornos]**, elija un entorno existente en la lista desplegable o seleccione **[!UICONTROL Agregar entorno]** para crear uno.
1. Abra **[!UICONTROL Configuración]** para el entorno seleccionado.
1. Escriba **[!UICONTROL ID de cliente]** y **[!UICONTROL Secreto de cliente]** de [LaunchPoint](#create-or-select-a-launchpoint-service), la **[!UICONTROL URL de identidad de Marketo Engage]** y la **[!UICONTROL URL base de la API de REST de Marketo Engage]** (el host base de [Servicios web](#note-your-marketo-rest-api-base-url)) para la URL de identidad de Marketo Engage &#x200B;y la URL base de la API de REST de Marketo Engage.
1. Haga clic en **[!UICONTROL Implementar]**. Cuando la implementación se realiza correctamente, la acción cambia a **[!UICONTROL Anular la implementación]**.

### Actualizar configuración

Para cambiar los valores de configuración de un entorno, **[!UICONTROL Anule la implementación]** primero, actualice los campos y, a continuación, **[!UICONTROL Implemente]** de nuevo.

### Configuración de Workspace (opcional)

Puede omitir este paso si desea utilizar el espacio de trabajo predeterminado. De manera predeterminada, los campos **Workspace ID** y **Tamaño de página de lista de plantilla** están preconfigurados.

Sin embargo, si necesita recuperar plantillas de un espacio de trabajo diferente:

1. En Marketo, vaya a **[!UICONTROL Admin]** → **[!UICONTROL Security]** → **[!UICONTROL Workspaces y particiones]**.
1. La columna **Workspace ID** está oculta de manera predeterminada. Para habilitarlo, haga clic con el botón derecho en la fila de encabezado (donde se muestran los nombres de columna).
1. Seleccionar **[!UICONTROL columnas]**.
1. Habilitar **[!UICONTROL ID]** de la lista.
   ![Espacios de trabajo y particiones con la columna Workspace ID habilitada](/help/extensibility/marketo-workspace-id.png){width="80%"}

Una vez que esté visible, usa el **Workspace ID** apropiado para tu configuración.

## Acceso a plantillas de Marketo en GenStudio

Una vez instalado y configurado Marketo para GenStudio, aparecerá la pestaña **[!UICONTROL Plantillas de Marketo]** al crear una experiencia de **Correo electrónico** en GenStudio. Utilice esa pestaña para examinar las plantillas de Marketo Engage.

>[!IMPORTANT]
>
>Cree correos electrónicos bajo el flujo de experiencia **correo electrónico estándar** en GenStudio for Performance Marketing. Esta integración NO admite correos electrónicos creados con la nueva experiencia del editor de correo electrónico.

![Configuración de Exchange con credenciales de Marketo](/help/extensibility/marketo-exchange-configuration.png){width="80%"}

## Resolución de problemas

### La pestaña Plantillas de Marketo no está visible

* Confirme que la aplicación está **aprobada** en Exchange y que el entorno está **implementado** con una ID de cliente, un secreto de cliente y URL base de Marketo válidos.
* Pida al administrador que verifique que se usó el acceso de **Marketo Product Admin** al crear credenciales.

### Las plantillas no se cargan

* Vuelva a cargar la página o cierre la sesión y vuelva a iniciarla en GenStudio.
* En el panel de herramientas para desarrolladores de navegador **[!UICONTROL Red]**, busque las llamadas de API fallidas a su instancia de Marketo y compruebe que la URL base de REST coincida con **[!UICONTROL Servicios web]** en Marketo (sin ruta adicional después del host).

### Error &quot;No se han encontrado plantillas&quot;

Si la extensión se instala correctamente y la pestaña Plantillas de Marketo está visible pero muestra &quot;No se han encontrado plantillas&quot;, el problema puede deberse a que la aplicación ha superado los límites de tamaño al procesar las plantillas, lo que provoca un bloqueo.
Para resolver esto:

1. Anule la implementación de la aplicación desde Exchange.
1. Reduzca el tamaño de página de la lista de plantillas (por ejemplo, establézcalo en 1 o 2).
1. Vuelva a implementar la aplicación.
