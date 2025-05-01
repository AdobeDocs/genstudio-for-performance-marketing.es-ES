---
title: Conectar medios de pago
description: Conecte una cuenta de canal para activar y supervisar sus anuncios y medios con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
source-git-commit: cf4be61925761c9630cb8ea5c995d017b3938a31
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 0%

---

# Conectar cuentas de medios de pago

_[!DNL Data connectors]_habilita la integración perfecta entre GenStudio for Performance Marketing y sus cuentas de red de medios de pago. Al conectarse a cuentas de canales de terceros, puede intercambiar datos esenciales, como métricas de rendimiento de campañas en [[!DNL Insights]](/help/user-guide/insights/overview.md), y puede entregar nuevas ubicaciones de anuncios con [[!DNL Activate]](/help/user-guide/activation/overview.md). Esta integración permite a GenStudio for Performance Marketing administrar los contenidos y los anuncios a la vez que recibe información valiosa, como impresiones, clics y conversiones, de las campañas activas.

**Para conectarse a una cuenta de medios pagados**:

1. Haga clic en los puntos suspensivos **[!UICONTROL ... Más]** en la navegación inferior izquierda.

1. Seleccione **[!UICONTROL Configuración]** con el icono de engranaje.

1. En _[!UICONTROL Configuración]_, elija un tipo de conector en la sección _[!UICONTROL Conectores de datos]_ y haga clic en **[!UICONTROL Conectar]**.

   De manera opcional, si hay cuentas conectadas, puede hacer clic en _cuentas conectadas_ para ver una lista de nombres de cuentas, detalles y estado.

1. Vea el [tipo de conector](#connector-types) que seleccionó, revise los requisitos previos y continúe con los pasos de conexión.

## Conexiones de medios de pago

GenStudio for Performance Marketing admite varios tipos de conectores para integrarlos con las plataformas de marketing que prefiera. Cada tipo de conector tiene requisitos previos específicos y pasos de configuración que se deben completar para que la conexión se realice correctamente.

### Google Campaign Manager 360 connect

>[!BEGINSHADEBOX]

**Requisitos previos**:

- Cuenta de Google Campaign Manager 360
- Elimine los bloqueadores de ventanas emergentes del explorador

>[!ENDSHADEBOX]

**Para conectar una cuenta de Google Campaign Manager 360**:

1. En la sección _Conectores de datos_, haga clic en **[!UICONTROL Conectar]** en la tarjeta de _Google Campaign Manager 360_.

1. Inicie sesión en su cuenta de Google Campaign Manager 360.

   Es posible que tenga que quitar los bloqueadores de ventanas emergentes y, a continuación, usar **[!UICONTROL Actualizar]** para intentarlo de nuevo.

1. Lea los términos y condiciones y haga clic en **[!UICONTROL Permitir]** para conceder acceso.

1. En la vista _[!UICONTROL Google Campaign Manager 360]_, seleccione uno o más anunciantes y haga clic en **[!UICONTROL Seleccionar]**.

La vista de _[!UICONTROL cuentas de Google Campaign Manager 360]_ enumera `Account name`, `Added by`, `Date added` y `Status`. Use **[!UICONTROL Agregar cuenta]** para agregar más cuentas a la lista.

### Meta ads connect

Al conectar el perfil de _Meta Business_ a GenStudio for Performance Marketing, se garantiza un acceso sin problemas a los datos de publicidad de las páginas de empresa, las cuentas de Meta Ads y otros recursos Meta.

>[!BEGINSHADEBOX]

**Requisitos previos**:

- Inicio de sesión de Facebook/Meta que puede acceder a todos los servicios Meta, como la cuenta de Meta Ads y el perfil comercial de Facebook
- Acceso a la cuenta de Meta ads con nivel de permiso `View performance` para acceder a informes y ver anuncios, incluyendo lo siguiente
   - Permisos necesarios para usar con [!DNL Insights]:

      - `pages_show_list`
      - `ads_read`
      - `ads_management`
      - `pages_read_engagement`

   - Permisos necesarios para usar con [!DNL Activate]:

      - `ads_management`
      - `ads_read`
      - `business_management`
      - `instagram_basic`
      - `instagram_content_publish`
      - `pages_manage_ads`
      - `pages_manage_posts`
      - `pages_show_list`

- Elimine los bloqueadores de ventanas emergentes del explorador

>[!ENDSHADEBOX]

**Para conectar una cuenta de Meta ads**:

1. En la sección _Conectores de datos_, haga clic en **[!UICONTROL Conectar]** en la tarjeta _Meta Ads_.

1. Inicie sesión en su cuenta de Facebook.

   Es posible que tenga que quitar los bloqueadores de ventanas emergentes y, a continuación, usar **[!UICONTROL Actualizar]** para intentarlo de nuevo.

1. Siga las instrucciones de autenticación de Facebook, verifique la información de la cuenta y haga clic en **[!UICONTROL Continuar como...]**

1. En _[!UICONTROL Inicio de sesión de Facebook para empresas]_ (símbolo Meta a Adobe), siga los siguientes pasos para conceder acceso a GenStudio for Performance Marketing:

   - Seleccione uno o varios perfiles de metaempresa y haga clic en **[!UICONTROL Continuar]**
   - Seleccione una o más Meta Pages y haga clic en **[!UICONTROL Continuar]**
   - Seleccione una o más cuentas de Instagram y haga clic en **[!UICONTROL Continuar]**
   - Revise las selecciones y haga clic en **[!UICONTROL Guardar]**

1. Una vez que hayas verificado que tu cuenta está conectada, haz clic en **[!UICONTROL Obtenerla]**.

   Este paso garantiza que GenStudio for Performance Marketing obtenga acceso a todos los anuncios, metadatos y métricas para obtener un rendimiento óptimo.

1. En _[!UICONTROL Meta Ads]_, seleccione una o más cuentas para incluirlas en [!DNL Insights] y haga clic en **[!UICONTROL Seleccionar]**.

1. Una vez que reciba una confirmación de _Plataforma conectada_, haga clic en **[!UICONTROL Ver cuentas]**.

   La vista de _[!UICONTROL cuentas de Meta Ads]_ enumera `Account name`, `Added by`, `Date added` y `Status`.

Use **[!UICONTROL Agregar cuenta]** para agregar más cuentas a la lista. El flujo de autorización puede diferir ligeramente cuando agrega cuentas vinculadas al mismo perfil de MetaBusiness. Solo selecciona las nuevas cuentas de Meta Ads durante el proceso de conexión.

## Ingesta de datos

Inicialmente, GenStudio for Performance Marketing importa los últimos seis meses de datos históricos. Esta práctica garantiza el acceso inmediato a perspectivas relevantes para analizar tendencias, evaluar el rendimiento y tomar decisiones informadas. El proceso de ingesta puede tardar entre uno y cinco días según el volumen de datos de su cuenta.

>[!BEGINSHADEBOX]

**Directiva de retención e ingesta de datos**

GenStudio for Performance Marketing retiene los datos de canal durante 13 meses. Esta política de retención incluye los 6 meses de datos introducidos durante la conexión inicial, lo que garantiza un análisis y unos informes de datos históricos completos.

>[!ENDSHADEBOX]
