---
title: Roles y permisos de usuarios de Adobe GenStudio for Performance Marketing
description: Obtenga información sobre las funciones de usuario y los permisos de GenStudio for Performance Marketing.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
role: Admin
exl-id: 33ebcf9c-e5f8-4011-b449-5f73d151f221
source-git-commit: 8a5d15df7a347c4ee7767610fc9bb23fc7b71db4
workflow-type: tm+mt
source-wordcount: '1133'
ht-degree: 7%

---

# Funciones de usuario y permisos

La creación e implementación de campañas de marketing modernas requieren la colaboración entre partes interesadas con diversas responsabilidades y conjuntos de habilidades. _Las funciones de usuario_ controlan el acceso de las partes interesadas a las numerosas funcionalidades de GenStudio for Performance Marketing. La función de usuario asignada determina las tareas que puede realizar con esta plataforma. Un administrador del sistema de Adobe le asigna una función en el perfil de producto de GenStudio en Adobe Admin Console. El correo electrónico de bienvenida identifica su función asignada.

>[!NOTE]
>
>Antes de aprovisionar usuarios en estas funciones, se debe designar un administrador del sistema de Adobe en Adobe Admin Console para que realice tareas de configuración únicas. Esta función de administrador de Adobe solo funciona en el contexto de Adobe Admin Console. No tiene función en la interfaz de la plataforma GenStudio for Performance Marketing. Un administrador del sistema de Adobe que necesite derechos de administrador del sistema debe aprovisionarse como administrador del sistema de GenStudio en Adobe Admin Console. Consulte [Aprovisionar GenStudio for Performance Marketing](product-provisioning.md).

## Administrador del sistema de Adobe frente a administrador del sistema de GenStudio

Estos títulos de funciones de usuario pueden parecer similares, pero identifican funciones únicas que proporcionan autorizaciones en entornos diferentes.

**Los administradores del sistema de Adobe** tienen privilegios de usuario avanzado en Adobe Admin Console y realizan todas las tareas de administración de usuarios, como agregar o eliminar usuarios. Esta función de administrador del sistema no proporciona privilegios en la aplicación de GenStudio for Performance Marketing, lo que explica por qué los administradores del sistema de Adobe no necesitan una licencia para GenStudio. Los administradores del sistema de Adobe suelen utilizar Admin Console para agregar y eliminar cuentas de usuario de implementaciones de GenStudio y asignar o quitar derechos o permisos de usuarios individuales o grupos de usuarios.

**Los administradores del sistema de GenStudio** son usuarios avanzados dentro de GenStudio for Performance Marketing, pero no tienen permiso para realizar tareas en Adobe Admin Console. Esta función de administrador del sistema requiere una licencia de producto de GenStudio y corresponde a un usuario avanzado en la [descripción del producto de Adobe GenStudio for Performance Marketing](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html). Los administradores del sistema de GenStudio tienen derecho total a las funciones de GenStudio for Performance Marketing, incluidas [!DNL Brands], [!DNL Persona] y [!DNL Product], creación, eliminación, actualización y publicación. [Descripción del producto Adobe GenStudio for Performance Marketing](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html) explica cómo se relacionan las funciones de usuario de GenStudio con las licencias de productos.

Consulte [Funciones administrativas](https://helpx.adobe.com/enterprise/using/admin-roles.html#enterprise) en la _Guía de administración de empresas y equipos_.

## Derechos

_Derechos_ conceden permiso para realizar tareas específicas y acceder a recursos protegidos. Los derechos o permisos se definen en la función de usuario dentro del perfil del producto y los usuarios reciben estos derechos cuando se les asigna esa función.

>[!IMPORTANT]
>
>No agregue perfiles de producto nuevos ni edite ni elimine los existentes. Modificar los perfiles de producto predeterminados puede afectar gravemente a la implementación de GenStudio for Performance Marketing.

## Funciones de los usuarios

Existen tres tipos de funciones de usuario de GenStudio for Performance Marketing que admiten esta diversidad de funciones organizativas. Los derechos se adaptan a cada uno de estos tipos de usuarios y respaldan las responsabilidades de cada usuario en la organización de marketing. Estos tres tipos de funciones de usuario son:

* **Los editores de GenStudio** utilizan las capacidades de IA generativa de GenStudio for Performance Marketing para crear recursos de campañas de marketing, solicitar la revisión y aprobación del contenido y publicar borradores aprobados de este contenido. Todos los usuarios de GenStudio for Performance Marketing pueden acceder a un recurso y utilizarlo una vez que su editor lo haya guardado en [!DNL Content]. Los editores de GenStudio son usuarios avanzados en GenStudio for Performance Marketing.

* **Los colaboradores de GenStudio** son la gama más amplia de usuarios de GenStudio for Performance Marketing. Los colaboradores pueden ver y aprobar contenido, y son una parte esencial del flujo de trabajo, que garantiza que el contenido que genere coincida con las necesidades y los estándares de su organización. Los colaboradores de GenStudio son _usuarios colaboradores_ en GenStudio for Performance Marketing.

* **Administradores del sistema de GenStudio** tienen el conjunto más amplio de derechos o permisos dentro de GenStudio for Performance Marketing. Los administradores de sistemas realizan la tarea de incorporación esencial de establecer las barreras fundamentales para la creación y la implementación de recursos de la campaña. Los administradores del sistema implementan estas protecciones cargando información específica de la marca y de la organización, como [directrices de marca](./guidelines/overview.md). Los administradores del sistema tienen permiso para crear y publicar [!DNL Brands], pero no tienen privilegios de administración de usuarios. Los administradores de sistemas de GenStudio son usuarios avanzados en GenStudio for Performance Marketing.

### Editores de GenStudio

_Los editores_, o los creadores de contenido, tienen los permisos principales necesarios para crear los recursos de GenStudio for Performance Marketing [!DNL Brands], [!DNL Campaigns] y [!DNL Content]. Estos usuarios avanzados también pueden editar y eliminar los recursos que han creado. GenStudio for Performance Marketing permite crear rápidamente cientos de fragmentos de contenido. Estos usuarios pueden generar fragmentos de contenido o experiencias completas que organicen fragmentos discretos de contenido aprobado para satisfacer las necesidades de campañas de marketing específicas.

Los editores interactúan con las tecnologías de IA generativa de GenStudio for Performance Marketing mediante _mensajes_. El cajón de mensajes del lienzo proporciona herramientas para colocar mensajes en el contexto de las directrices de una campaña específica. Como resultado, la calidad y el éxito del contenido generado dependen parcialmente de la calidad de las directrices de marca que su organización ha cargado y de la especificidad del mensaje. Consulte [Escribir mensajes efectivos](effective-prompts.md).

La siguiente tabla muestra los permisos de editor predeterminados:

| Función | Crear | Actualizar | Eliminar | Ver |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | no | no | no | sí |
| [!DNL Campaigns] | sí | sí | sí | sí |
| [!DNL Content] | sí | sí | sí | sí |
| [!DNL Create] | sí | sí | sí | sí |
| [!DNL Insights] | solo puede configurar conectores |    |     | sí |
| [!DNL Personas] | sí | sí* | sí* | sí |
| [!DNL Products] | sí | sí* | sí* | sí |
| [!DNL Reviews and approvals] | sí | sí | sí | sí |
| [!DNL Templates] | no | no | no | sí |

Los editores pueden editar y eliminar [!DNL Personas] y [!DNL Products] que hayan creado.

Los administradores del sistema de GenStudio pueden dar permiso a los editores para editar y eliminar un(a) [!DNL Brand].

### Colaboradores de GenStudio

_Los colaboradores_ pueden ver los recursos en GenStudio for Performance Marketing, pero no crearlos, editarlos o eliminarlos. Por ejemplo, los colaboradores ven el mensaje &quot;*No tiene acceso a este contenido*&quot; cuando intentan obtener acceso a [[!DNL Create]](/help/user-guide/create/overview.md).

Los colaboradores incluyen partes interesadas que son esenciales para el éxito del proceso de revisión y aprobación del contenido, pero que no necesitan crear ni editar contenido directamente. Los expertos legales y los gerentes de creativos son ejemplos de colaboradores potenciales. Los colaboradores de GenStudio for Performance Marketing pueden tener permiso para crear y ver recursos en otros productos de Creative Cloud.

En la tabla siguiente se muestran los permisos de colaborador predeterminados:

| Función | Crear | Actualizar | Eliminar | Ver |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | no | no | no | sí |
| [!DNL Campaigns] | no | no | no | sí |
| [!DNL Content] | no | no | no | sí |
| [!DNL Create] | no | no | no | sí |
| [!DNL Insights] | no | no | no | sí |
| [!DNL Personas] | no | no | no | sí |
| [!DNL Products] | no | no | no | sí |
| [!DNL Reviews and approvals] | no | no | no | sí |
| [!DNL Templates] | no | no | no | sí |

### administradores del sistema de GenStudio

_Administradores del sistema de GenStudio_ tienen el conjunto más potente de permisos dentro de GenStudio for Performance Marketing. Estos usuarios avanzados realizan la tarea de incorporación esencial de establecer las barreras fundamentales para la creación y la implementación de recursos de la campaña. Los administradores del sistema implementan estas protecciones cargando información específica de la marca y de la organización, como [directrices de marca](./guidelines/overview.md). Los administradores del sistema tienen permiso para crear y publicar [!DNL Brands], pero no tienen privilegios de administración de usuarios.

En la tabla siguiente se muestran los permisos predeterminados del administrador del sistema:

| Función | Crear | Actualizar | Eliminar | Ver |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | sí | sí | sí | sí |
| [!DNL Campaigns] | sí | sí | sí | sí |
| [!DNL Content] | sí | sí | sí | sí |
| [!DNL Insights] | sí | sí | sí | sí |
| [!DNL Personas] | sí | sí | sí | sí |
| [!DNL Products] | sí | sí | sí | sí |
| [!DNL Reviews and approvals] | sí | sí | sí | sí |
| [!DNL Templates] | sí | sí | sí | sí |

Los administradores del sistema también pueden cargar plantillas.

Consulte [Introducción a Adobe GenStudio for Performance Marketing](get-started.md) para obtener una descripción general de las tareas de configuración preliminares.
