---
title: Asignar  [!DNL Brand] permisos
description: Obtenga información acerca de la asignación de derechos para creadores y editores de GenStudio for Performance Marketing [!DNL Brand] s.
level: Intermediate
feature: Brands Service, Generative AI
source-git-commit: 3c391753ebd0d19ad7dcb17870915eeccc55cc05
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 1%

---

# Asignar permisos de [!DNL Brand]

De manera predeterminada, los administradores del sistema de GenStudio pueden crear y editar [!DNL Brands]. Las funciones de editor de contenido y colaborador tienen permisos de edición y creación, pero es posible que no requieran derechos de administración del sistema. Para conceder a los editores de contenido y a los colaboradores estos derechos relacionados con [!DNL Brand], un administrador del sistema de Adobe debe realizar algunas tareas de configuración adicionales en Adobe Admin Console. Consulte [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html#Overview) en la _guía de administración de empresas y equipos_.

Añadir usuarios y grupos de usuarios son tareas básicas comunes a todos los productos de Adobe con autorizaciones que se administran mediante el Admin Console. Consulte [Usuarios de Adobe Admin Console](https://helpx.adobe.com/es/enterprise/using/users.html) en la _Guía de administración de equipos y empresas_ para obtener una descripción general de la administración de usuarios y los procedimientos para agregar usuarios y grupos de usuarios.

## Paso 1: Crear un grupo de usuarios

**Para crear un grupo de usuarios**:

1. Inicie sesión en el Admin Console y navegue hasta **[!UICONTROL Usuarios]** > **[!UICONTROL Grupos de usuarios]**.

1. Haga clic en **[!UICONTROL Nuevo grupo de usuarios]**. Se abre la ventana emergente _Crear un nuevo grupo de usuarios_.

1. Agregue un nombre de grupo de usuarios informativo al campo **[!UICONTROL Nombre de grupo de usuarios]** para identificar el propósito del nuevo grupo. Por ejemplo, &quot;Administradores de marca&quot;.

1. Opcionalmente, añada una descripción del grupo y su propósito.

1. Haga clic en **[!UICONTROL Guardar]**. El Admin Console abre la ventana emergente _Nuevo grupo_ con el nombre del grupo recién creado.

Consulte [Administrar grupos de usuarios](https://helpx.adobe.com/es/enterprise/using/user-groups.html) en la _Guía de administración de empresas y equipos_.

## Paso 2: Asignar un perfil de administrador del sistema de GenStudio al grupo de usuarios

Una vez que haya creado un nuevo grupo de usuarios y agregado usuarios, puede asignar el perfil **administrador del sistema de Adobe GenStudio** a este grupo. Las autorizaciones asociadas al perfil asignado conceden a todos los usuarios de este grupo permisos de GenStudio [!DNL Brands] (crear, actualizar y eliminar marcas).

**Para asignar un perfil al grupo de usuarios**:

1. Vaya al grupo de usuarios recién creado y haga clic en la ficha _Perfiles de producto asignados_.

1. En la ficha _Perfiles de producto asignados_, haga clic en **[!UICONTROL Asignar perfil]**. Se abre la ventana emergente _Asignar productos y perfiles_.

1. Seleccione `Adobe GenStudio` de la lista _Seleccionar productos_.

1. Haga clic en **[!UICONTROL Aplicar]**. Se abre la ventana emergente _Seleccionar perfiles de producto_, que muestra los perfiles de producto asociados con el Adobe GenStudio.

1. Seleccione `Adobe GenStudio system manager`.

1. Haga clic en **[!UICONTROL Aplicar]**. Se abre la ventana emergente _Asignar productos y perfiles_, que muestra el perfil de producto para el grupo de usuarios recién creado.

1. Haga clic en **[!UICONTROL Guardar]**.

Consulte [Asignar perfiles de producto a grupos de usuarios](https://helpx.adobe.com/es/enterprise/using/user-groups.html) en la _Guía de administración de empresas y equipos_.

## Paso 3: Crear un proyecto [!DNL Brands]

Un _proyecto_ proporciona una ubicación de almacenamiento donde determinados usuarios pueden guardar recursos, en este caso, [!DNL Brands] recursos.

**Para crear un proyecto [!DNL Brands] desde la ficha _Almacenamiento_**:

1. Vaya a la ficha _Almacenamiento_ en el Admin Console.

1. Haga clic en **[!UICONTROL Proyectos]** en la navegación lateral. Se abre la pestaña _Proyectos_.

1. Haga clic en **[!UICONTROL Crear proyecto]**. Se abre la ventana emergente _Nuevo proyecto_.

1. Escriba `Adobe GenStudio Brands` en el campo de nombre de proyecto. Escriba este nombre de proyecto exactamente como se muestra aquí. No incluya espacios adicionales ni cambie las mayúsculas y minúsculas.

1. Haga clic en **[!UICONTROL Crear]**. Se abre la ventana emergente _Invitar al proyecto_.

Consulte [Administrar proyectos](https://helpx.adobe.com/enterprise/using/projects-in-business-storage.html) en la _Guía de administración de empresas y equipos_.

## Paso 4: Invitar al grupo de usuarios al proyecto

Ya está listo para agregar el grupo de usuarios que acaba de crear al proyecto `Adobe GenStudio [!DNL Brands]`.

**Para invitar al grupo de usuarios al proyecto recién creado**:

1. En la ventana emergente _Invitar al proyecto_, agregue el grupo de usuarios que acaba de crear a este proyecto.

1. Elija la opción de permisos **Puede editar**.

1. Haga clic en **[!UICONTROL Invitar]**.

## Paso 5: Agregar usuarios al grupo de usuarios

Para asignar a los usuarios el permiso para crear, editar y publicar [!DNL Brands], agréguelos al grupo de usuarios recién creado.

**Para agregar usuarios al grupo de usuarios**:

1. Desde el _Admin Console_, vaya a **[!UICONTROL Usuarios]** > **[!UICONTROL Grupos de usuarios]**.

1. Seleccione el nombre del grupo de usuarios que creó anteriormente. Se abre la ventana emergente _Agregar usuarios a este grupo de usuarios_.

1. Agregue un usuario nuevo o existente por nombre de usuario o dirección de correo electrónico. Obtenga información acerca de la administración de grupos de usuarios en [Administrar grupos de usuarios](https://helpx.adobe.com/es/enterprise/using/user-groups.html) en la _Guía de administración de empresas y equipos_.

A los usuarios se les conceden los permisos de creación, edición y publicación de [!DNL Brand] de los administradores del sistema de Adobe GenStudio cuando se agregan al grupo. Los usuarios también reciben una invitación automatizada por correo electrónico para editar el proyecto de Adobe GenStudio for Performance Marketing [!DNL Brands].