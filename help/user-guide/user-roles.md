---
title: Roles y permisos de usuarios de Adobe GenStudio for Performance Marketing
description: Obtenga información sobre las funciones de usuario y los permisos de GenStudio for Performance Marketing.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
source-git-commit: 3e9a2a4f42ba79389691705c571bf6bbd0b990c5
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 2%

---

# Funciones de usuario y permisos

La creación e implementación de campañas de marketing modernas requieren la colaboración entre partes interesadas con diversas responsabilidades y conjuntos de habilidades. _Las funciones de usuario_ controlan el acceso de las partes interesadas a las numerosas funcionalidades de GenStudio for Performance Marketing. La función de usuario asignada determina las tareas que puede realizar con esta plataforma. Un administrador del sistema de Adobe le asigna una función en el perfil de producto de GenStudio en Adobe Admin Console. El correo electrónico de bienvenida identifica su función asignada.

>[!NOTE]
>
>Antes de aprovisionar a cualquier usuario en estas funciones, se debe designar un administrador del sistema de Adobe en Adobe Admin Console para realizar tareas de configuración únicas. Esta función de administrador de Adobe solo funciona en el contexto de Adobe Admin Console. No tiene función en la interfaz de la plataforma GenStudio for Performance Marketing. Un administrador del sistema de Adobe que necesite derechos de administrador del sistema debe aprovisionarse como administrador del sistema de GenStudio en Adobe Admin Console. Consulte [Aprovisionar GenStudio for Performance Marketing](product-provisioning.md).

## Derechos

_Derechos_ conceden permiso para realizar tareas específicas y acceder a recursos protegidos. Los derechos se definen en la función de usuario dentro del perfil de producto y los usuarios reciben estos derechos cuando se les asigna esa función.

## Funciones de los usuarios

Existen tres tipos de funciones de usuario de GenStudio for Performance Marketing que admiten esta diversidad de funciones organizativas. Los permisos se adaptan a cada uno de estos tipos de usuarios y admiten las responsabilidades de cada usuario en la organización de marketing. Estos tres tipos de funciones de usuario son:

* **Los editores de GenStudio** utilizan las capacidades de IA generativa de GenStudio for Performance Marketing para crear recursos de campañas de marketing, solicitar la revisión y aprobación del contenido y publicar borradores aprobados de este contenido. Todos los usuarios de GenStudio for Performance Marketing pueden acceder a un recurso y utilizarlo una vez que su editor lo haya guardado en [!DNL Content].

* **Los colaboradores de GenStudio** son la gama más amplia de usuarios de GenStudio for Performance Marketing. Los colaboradores pueden ver y aprobar contenido, y son una parte esencial del flujo de trabajo, que garantiza que el contenido que genere coincida con las necesidades y los estándares de su organización.

* **Administradores del sistema de GenStudio** tienen el conjunto más amplio de permisos dentro de GenStudio for Performance Marketing. Los administradores de sistemas realizan la tarea de incorporación esencial de establecer las barreras fundamentales para la creación y la implementación de recursos de la campaña. Los administradores del sistema implementan estas protecciones cargando información específica de la marca y de la organización, como [directrices de marca](./guidelines/overview.md). Los administradores del sistema tienen permiso para crear y publicar [!DNL Brands], pero no tienen privilegios de administración de usuarios.

### Editores de GenStudio

_Los editores_, o los creadores de contenido, tienen los permisos principales necesarios para crear los recursos de GenStudio for Performance Marketing [!DNL Brands], [!DNL Campaigns] y [!DNL Content]. También pueden editar y eliminar los recursos que han creado. GenStudio for Performance Marketing permite crear rápidamente cientos de fragmentos de contenido. Estos usuarios pueden generar fragmentos de contenido o experiencias completas que organicen fragmentos discretos de contenido aprobado para satisfacer las necesidades de campañas de marketing específicas.

Los editores interactúan con las tecnologías de IA generativa de GenStudio for Performance Marketing mediante _mensajes_. El cajón de mensajes del lienzo proporciona herramientas para colocar mensajes en el contexto de las directrices de una campaña específica. Como resultado, la calidad y el éxito del contenido generado dependen parcialmente de la calidad de las directrices de marca que su organización ha cargado y de la especificidad del mensaje. Consulte [Escribir mensajes efectivos](effective-prompts.md).

La siguiente tabla muestra los permisos de editor predeterminados:

| Funcionalidad | Crear | Actualizar | Eliminar | Ver |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | no | no | no | yes |
| [!DNL Campaigns] | yes | yes | yes | yes |
| [!DNL Content] | yes | yes | yes | yes |
| [!DNL Create] | yes | yes | yes | yes |
| [!DNL Insights] | solo puede configurar conectores de publicidad |    |     | yes |
| [!DNL Personas] | yes | sí* | sí* | yes |
| [!DNL Products] | yes | sí* | sí* | yes |
| [!DNL Reviews and approvals] | yes | yes | yes | yes |

Los editores pueden editar y eliminar [!DNL Personas] y [!DNL Products] que hayan creado.

Los administradores del sistema de GenStudio pueden dar permiso a los editores para editar y eliminar un(a) [!DNL Brand].

### Colaboradores de GenStudio

_Los colaboradores_ pueden ver los recursos en GenStudio for Performance Marketing, pero no crearlos, editarlos o eliminarlos. Los colaboradores incluyen partes interesadas que son esenciales para el éxito del proceso de revisión y aprobación del contenido, pero que no necesitan crear ni editar contenido directamente. Los expertos legales y los gerentes de creativos son ejemplos de colaboradores potenciales. Los colaboradores de GenStudio for Performance Marketing pueden tener permiso para crear y ver recursos en otros productos de Creative Cloud.

En la tabla siguiente se muestran los permisos de colaborador predeterminados:

| Funcionalidad | Crear | Actualizar | Eliminar | Ver |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | no | no | no | yes |
| [!DNL Campaigns] | no | no | no | yes |
| [!DNL Content] | no | no | no | yes |
| [!DNL Create] | no | no | no | yes |
| [!DNL Insights] | no | no | no | yes |
| [!DNL Personas] | no | no | no | yes |
| [!DNL Products] | no | no | no | yes |
| [!DNL Reviews and approvals] | no | no | no | yes |

### administradores del sistema de GenStudio

_Administradores del sistema de GenStudio_ tienen el conjunto más potente de permisos dentro de GenStudio for Performance Marketing. Los administradores de sistemas realizan la tarea de incorporación esencial de establecer las barreras fundamentales para la creación y la implementación de recursos de la campaña. Los administradores del sistema implementan estas protecciones cargando información específica de la marca y de la organización, como [directrices de marca](./guidelines/overview.md). Los administradores del sistema tienen permiso para crear y publicar [!DNL Brands], pero no tienen privilegios de administración de usuarios.

En la tabla siguiente se muestran los permisos predeterminados del administrador del sistema:

| Funcionalidad | Crear | Actualizar | Eliminar | Ver |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | yes | yes | yes | yes |
| [!DNL Campaigns] | yes | yes | yes | yes |
| [!DNL Content] | yes | yes | yes | yes |
| [!DNL Insights] | yes | yes | yes | yes |
| [!DNL Personas] | yes | yes | yes | yes |
| [!DNL Products] | yes | yes | yes | yes |
| [!DNL Reviews and approvals] | yes | yes | yes | yes |

Consulte [Introducción a Adobe GenStudio for Performance Marketing](get-started.md) para obtener una descripción general de las tareas de configuración preliminares.
