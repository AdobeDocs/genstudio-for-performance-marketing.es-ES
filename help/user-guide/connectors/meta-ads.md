---
title: Conectar con Meta Ads
description: Conecte una cuenta de Meta Ads para activar y controlar los anuncios y los contenidos con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
recommendations: noDisplay
feature: Reporting and Insights
exl-id: 78110edf-947b-4e05-a3f1-de4b1eabda44
source-git-commit: dce3d9bbf3ed2d26872b324c04ab7e78bbb034dc
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# Conectar con Meta Ads

En esta página se explica cómo conectar y administrar su cuenta de perfil de Meta Ads a GenStudio for Performance Marketing para administrar campañas, exportar contenido y acceder a datos de publicidad para sus campañas activas.

>[!BEGINSHADEBOX]

**Requisitos previos**:

- Inicio de sesión de Facebook/Meta que puede acceder a todos los servicios de Meta
- _Control total_ sobre las cuentas de Meta Business Portfolio y Ad, que incluyen:
   - Administración de campañas
   - Ver rendimiento
   - Administrar maquetas de Creative Hub
   - Análisis avanzado
- Deshabilite los bloqueadores de ventanas emergentes del explorador
- Compruebe las asociaciones de páginas de cuentas de Instagram en Meta Business Manager antes de intentar establecer una conexión
- Confirmar acceso de administrador a todos los recursos que se están conectando

>[!ENDSHADEBOX]

## Conectar una cuenta de Meta Ads

1. Haga clic en **[!UICONTROL Más]** > **[!UICONTROL Configuración]**.

1. En la sección _Conectores de datos_, haga clic en **[!UICONTROL Conectar]** en la tarjeta de _Meta Ads_.

1. Inicie sesión en su cuenta de Facebook.

   Es posible que tenga que quitar los bloqueadores de ventanas emergentes y, a continuación, usar **[!UICONTROL Actualizar]** para intentarlo de nuevo.

1. Siga las instrucciones de autenticación de Facebook, verifique la información de la cuenta y haga clic en **[!UICONTROL Continuar como...]**

1. En _[!UICONTROL Inicio de sesión de Facebook para empresas]_ (símbolo de Meta a Adobe), siga los siguientes pasos para conceder acceso a GenStudio for Performance Marketing:

   - Seleccione uno o más perfiles de negocio de Meta y haga clic en **[!UICONTROL Continuar]**
   - Seleccione una o más páginas de Meta y haga clic en **[!UICONTROL Continuar]**
   - Seleccione una o más cuentas de Instagram y haga clic en **[!UICONTROL Continuar]**
   - Revise las selecciones y haga clic en **[!UICONTROL Guardar]**

     ![Revisar selecciones](/help/assets/meta/meta-review-selections.png "Revisar selecciones"){width="400" zoomable="yes"}

1. Una vez que hayas verificado que tu cuenta está conectada, haz clic en **[!UICONTROL Obtenerla]**.

   Este paso garantiza que GenStudio for Performance Marketing obtenga acceso a todos los anuncios, metadatos y métricas para obtener un rendimiento óptimo.

1. En _[!UICONTROL Meta Ads]_, seleccione una o más cuentas para incluirlas en [!DNL Insights] y haga clic en **[!UICONTROL Seleccionar]**.

1. Una vez que reciba una confirmación de _Plataforma conectada_, haga clic en **[!UICONTROL Ver cuentas]**.

   La vista de _[!UICONTROL cuentas de Meta Ads]_ enumera `Account name`, `Added by`, `Date added` y `Status`.

   ![Lista de cuentas de Meta](/help/assets/meta/meta-accounts-list.png "Lista de cuentas de Meta conectadas"){zoomable="yes"}

Use **[!UICONTROL Agregar cuenta]** para agregar más cuentas a la lista. El flujo de autorización puede diferir ligeramente cuando se agregan cuentas vinculadas al mismo perfil empresarial de Meta. Solo selecciona las nuevas cuentas de Meta Ads durante el proceso de conexión.

## Prácticas recomendadas de conexión

Para evitar errores, tenga en cuenta las siguientes prácticas recomendadas al configurar conexiones:

- [ ] Comience con una selección mínima de recursos (solo una página) para la conexión inicial
- [ ] Agregar cuentas de Instagram solo después de confirmar que el acceso a la página funciona
- [ ] Asegúrese de que las cuentas de Instagram estén correctamente asociadas con la página de Facebook seleccionada en Meta Business Manager
- [ ] Utilizar un enfoque por fases: primero establezca la conexión básica y luego expanda los recursos
- [ ]: compruebe los permisos de administración de todos los recursos antes de intentar la conexión

## Desconexión y solución de problemas de una integración con Meta Ads

A veces, una instancia de GenStudio for Performance Marketing está conectada a una cuenta de Meta Ads incorrectamente. Las configuraciones comunes que pueden causar problemas incluyen:

- Se selecciona una cuenta de Instagram sin seleccionar su página de Facebook asociada
- Permisos revocados para un usuario que realizó la conexión inicial

En estas situaciones, es mejor volver a conectar la cuenta de Meta Ad a la instancia de GenStudio for Performance Marketing. En primer lugar, el usuario debe quitar la integración de la aplicación directamente de su Meta Business Manager, lo que crea una pizarra limpia para restablecer los permisos. Esto requiere acceso de administrador a Meta Business Manager.

Estos pasos borran los permisos en caché y restablecen el flujo de integración:

1. Para obtener acceso a [Meta Business Manager](https://business.facebook.com), visite el sitio web de Facebook.
1. Inicie sesión con su cuenta de. La cuenta debe tener acceso de administrador a Business Manager.
1. Haga clic en el icono del engranaje de **[!UICONTROL Configuración]** en la esquina inferior izquierda para ir a la configuración de Business Portfolio.
1. En el menú de la izquierda, haga clic en **[!UICONTROL Integraciones]**.
1. Seleccione **[!UICONTROL Aplicaciones conectadas]**. Verá Adobe GenStudio en la lista de aplicaciones conectadas.
   ![Aplicaciones conectadas de Meta Business Manager](./meta-connected-apps.png "Panel de aplicaciones conectadas de Meta Business Manager")
1. Haga clic en el nombre de la aplicación.
1. Haga clic en **[!UICONTROL Quitar]**.
1. Confirme la eliminación cuando se le solicite.

Ahora puede volver a conectar sus cuentas de Meta Ad, perfiles de Instagram y páginas de Facebook.

## Problemas de conexión de cuenta de Instagram

Pueden producirse problemas cuando se seleccionan cuentas de Instagram sin conectar una página de Facebook asociada durante la configuración de la conexión. Esto puede causar errores como:

- &quot;No se pudo conectar con {Page_Name}&quot; o errores de conexión genérica.
- Tiempos de espera de conexión durante el flujo de inicio de sesión de Facebook para empresas.
- Se producen errores silenciosos cuando se seleccionan varios recursos.
- La conexión falla al seleccionar Instagram, Página y Añadir cuenta simultáneamente.

### Pasos de resolución:

1. Vaya a [Meta Business Manager](https://business.facebook.com) > Integraciones > Aplicaciones conectadas.
1. Elimine la integración existente de &quot;Adobe GenStudio&quot;, si la hay. Haga clic en **Quitar**.
1. Vuelva a GenStudio y vuelva a intentar el proceso de conexión.
1. Seleccione SOLAMENTE la página de Facebook de destino durante la conexión inicial.
1. NO seleccione la cuenta de Instagram durante el primer intento de conexión.
1. Compruebe que la conexión se haya realizado correctamente antes de añadir otros recursos.
1. Una vez que la conexión de Página sea estable, agregue las cuentas de Instagram por separado.


