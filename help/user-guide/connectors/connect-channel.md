---
title: Conéctese medios de pago
description: Conecte una cuenta de canal para activar y monitor sus anuncios y medios con Adobe Systems GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
source-git-commit: 2844914d25d9bc3a2be7f47d0cd7f26f7c921555
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Conectar cuentas medios de pago

_[!DNL Data connectors]_habilite integración optimizada entre GenStudio para Performance Marketing y sus cuentas de red medios de pago. Al conectarse a cuentas de terceros canal, puede intercambiar datos esencial, como métricas rendimiento de la campaña en [[!DNL Insights]](/help/user-guide/insights/overview.md), y puede entregar nuevas ubicaciones de anuncios con [[!DNL Activate]](/help/user-guide/activation/overview.md). Esta integración permite a GenStudio for Performance Marketing administrar sus medios y anuncios mientras recibe información valiosa, incluidas impresiones, clics y conversiones, de sus campañas activas.

**Para conectarse a un cuenta de medios de pago**:

1. Haga clic en los puntos suspensivos **[!UICONTROL ... Más]** en la parte inferior izquierda navegación.

1. Seleccione **[!UICONTROL Configuración]** con el icono de engranaje.

1. En _[!UICONTROL Configuración]_, elija un tipo de conector en la _[!UICONTROL sección Conectores de]_ datos y haga clic en **[!UICONTROL Conectar]**.

   Opcionalmente, si hay cuentas conectadas, puede hacer clic en _cuentas_ conectadas para vista una lista de cuenta nombres, detalles y estado.

1. Consulte el tipo](#connector-types) de [conector seleccionado, revise los requisitos previos y continúe con los pasos de conexión.

## Conexiones medios pago

GenStudio para Performance Marketing admite varios tipos de conectores para integrar con sus plataformas de marketing preferidas. Cada tipo de conector tiene requisitos previos específicos y pasos de configuración que completar para una conexión correcta.

### Meta ads connect

>[!BEGINSHADEBOX]

**Requisitos previos**:

- Facebook/Meta ads cuenta
- Acceso a meta anuncios cuenta con `View performance` nivel permiso para acceder a informes y ver anuncios
- Quitar bloqueadores de elemento emergente en su explorador

>[!ENDSHADEBOX]

**Para conectar una cuenta** de Meta anuncios:

1. En la _sección Conectores de_ datos, haga clic **[!UICONTROL en Conectar]** en el _tarjeta de Meta Ads_ .

1. Inicie sesión en su cuenta de Facebook.

   Es posible que tenga que quitar los bloqueadores de elemento emergente y, a continuación, usar **[!UICONTROL Actualizar]** para intentarlo de nuevo.

1. Siga las instrucciones de autenticación de Facebook.

1. En el elemento emergente de inicio de sesión de _[!UICONTROL Facebook para Empresa]_ (símbolo Meta a Adobe Systems), siga los pasos a seguir las siguientes selecciones.

   - Compruebe la información cuenta y haga clic en **[!UICONTROL Continuar como]**
   - Conceda acceso a páginas seleccionadas y haga clic en **[!UICONTROL Continuar]**
   - Conceda acceso a empresas seleccionadas y haga clic en **[!UICONTROL Continuar]**
   - Regístrate en una o varias cuentas de Instagram y haz clic en **[!UICONTROL Continuar]**
   - Revise las selecciones y haga clic en **[!UICONTROL Guardar]**

1. En el _[!UICONTROL vista Meta Ads]_ , seleccione una o varias cuentas y haga clic en **[!UICONTROL Seleccionar]**.

La _[!UICONTROL vista de cuentas]_ de Meta Ads incluye los , `Account name``Added by``Date added`, , y .`Status` Utilice **[!UICONTROL añadir cuenta]** para agregar más cuentas al lista.

## Ingesta de datos

Inicialmente, GenStudio para Performance Marketing importa los últimos seis meses de datos históricos. Esta práctica garantiza que tenga acceso inmediato a información relevante para analizar tendencias, evaluar el rendimiento y tomar decisiones informadas. El proceso de ingestión puede tardar de uno a cinco días, dependiendo del volumen de datos de su cuenta.

>[!BEGINSHADEBOX]

**Política de incorporación y retención de datos**

GenStudio para Performance Marketing conserva canal datos durante 13 meses. Este directiva de retención incluye los 6 meses de datos ingeridos durante la conexión inicial, lo que garantiza una datos históricos integral análisis y sistema de informes.

>[!ENDSHADEBOX]
