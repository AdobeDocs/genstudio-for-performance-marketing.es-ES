---
title: Introducción a Adobe GenStudio for Performance Marketing
description: Aprenda a configurar su GenStudio for Performance Marketing para generar nuevo contenido de marketing alineado con la marca.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: bcb03198-bbcb-45ae-af01-25c1e834b563
source-git-commit: 449c212ab167a6c126492e9becedf9318bfe08ee
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 1%

---

# Introducción a Adobe GenStudio for Performance Marketing

Adobe GenStudio for Performance Marketing es una plataforma completa para crear, evaluar y administrar experiencias de marketing que reflejen y se adhieran a la identidad de su marca.

El acceso de las partes interesadas a sus muchas capacidades está controlado por las _funciones de usuario_ asignadas. La función de usuario asignada determina las tareas que puede realizar en GenStudio for Performance Marketing. Un administrador del sistema de Adobe asigna sus permisos en el perfil de producto de GenStudio for Performance Marketing en Adobe Admin Console. El correo electrónico de bienvenida identifica su función asignada.

Si no tiene experiencia previa con herramientas generativas basadas en IA o simplemente siente curiosidad por conocer los principios básicos de GenStudio for Performance Marketing, consulte [Conceptos](concepts.md) y [Escribir mensajes efectivos](effective-prompts.md).

## Funciones de los usuarios

La creación e implementación de campañas de marketing modernas requieren la colaboración entre partes interesadas con diversas responsabilidades y conjuntos de habilidades.

Existen tres tipos de funciones de usuario de GenStudio for Performance Marketing que admiten esta diversidad de funciones organizativas. Los permisos se adaptan a cada uno de estos tipos de usuarios y admiten las responsabilidades de cada usuario en la organización de marketing.

**Los tres tipos de roles de usuario son**:

* **Los editores** utilizan las capacidades de IA generativa de GenStudio for Performance Marketing para crear recursos de campañas de marketing, solicitar la revisión y aprobación del contenido y publicar borradores aprobados de este contenido. Todos los usuarios de GenStudio for Performance Marketing pueden acceder a un recurso y utilizarlo una vez que su creador lo haya guardado en el Contenido.

* **Los colaboradores** son la gama más amplia de usuarios de GenStudio for Performance Marketing. Los colaboradores pueden ver y aprobar contenido, y son una parte esencial del flujo de trabajo, que garantiza que el contenido que genere coincida con las necesidades y los estándares de su organización.

* **Administradores del sistema** tienen el conjunto más amplio de permisos dentro de GenStudio for Performance Marketing. Los administradores de sistemas realizan la tarea de incorporación esencial de establecer las barreras fundamentales para la creación y la implementación de recursos de la campaña. Los administradores del sistema implementan estas protecciones cargando información específica de la marca y de la organización, como [directrices de marca](/help/user-guide/guidelines/overview.md). Los administradores del sistema de GenStudio for Performance Marketing tienen permiso para crear y publicar marcas, pero no tienen privilegios de administración de usuarios.

>[!NOTE]
>Antes de aprovisionar a cualquier usuario en estas funciones, se debe designar un administrador del sistema de Adobe en Adobe Admin Console para realizar tareas de configuración únicas. Esta función de administrador de Adobe solo funciona en el contexto de Adobe Admin Console. No tiene función en la interfaz de la plataforma GenStudio for Performance Marketing.

### Editores de GenStudio for Performance Marketing

**Los editores** tienen los permisos básicos necesarios para crear los recursos de GenStudio for Performance Marketing [!DNL Brands], [!DNL Campaigns] y [!DNL Content]. También pueden editar y eliminar los recursos que han creado. GenStudio for Performance Marketing permite crear rápidamente cientos de fragmentos de contenido. Estos usuarios pueden generar secciones de contenido o experiencias completas que organicen partes discretas de contenido aprobado para satisfacer las necesidades de campañas de marketing específicas.

Los editores interactúan con las tecnologías de IA generativa de GenStudio for Performance Marketing mediante _mensajes_. El cajón de mensajes del lienzo proporciona herramientas para colocar mensajes en el contexto de las directrices de una campaña específica. Como resultado, la calidad y el éxito del contenido generado dependen parcialmente de la calidad de las directrices de marca que su organización ha cargado y de la especificidad del mensaje.

Consulte [Escribir mensajes efectivos](effective-prompts.md).

La siguiente tabla muestra los permisos de editor predeterminados:

| Funcionalidad | Crear | Actualizar | Eliminar | Ver |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | no | no | no | yes |
| [!DNL Campaigns] | yes | yes | yes | yes |
| [!DNL Content] | yes | yes | yes | yes |
| [!DNL Insights] | solo puede configurar conectores de publicidad |    |     | yes |
| [!DNL Personas] | yes | yes | yes | yes |
| [!DNL Products] | yes | yes | yes | yes |
| [!DNL Reviews and approvals] | yes | yes | yes | yes |

### Colaboradores de GenStudio for Performance Marketing

**Los colaboradores** pueden ver los recursos en GenStudio for Performance Marketing, pero no crearlos, editarlos o eliminarlos. Los colaboradores incluyen partes interesadas que son esenciales para el éxito del proceso de revisión y aprobación del contenido, pero que no necesitan crear ni editar contenido directamente. Los expertos legales y los gestores de los creadores son ejemplos de colaboradores potenciales. Los colaboradores de GenStudio for Performance Marketing pueden tener permisos para crear y ver recursos en otros productos de Creative Cloud.

En la tabla siguiente se muestran los permisos de colaborador predeterminados:

| Funcionalidad | Crear | Actualizar | Eliminar | Ver |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | no | no | no | yes |
| [!DNL Campaigns] | no | no | no | yes |
| [!DNL Content] | no | no | no | yes |
| [!DNL Insights] | no | no | no | yes |
| [!DNL Personas] | no | no | no | yes |
| [!DNL Products] | no | no | no | yes |
| [!DNL Reviews and approvals] | no | no | no | yes |

### administradores del sistema de GenStudio for Performance Marketing

**administradores del sistema de GenStudio** completan las tareas iniciales que preparan a su organización para implementar GenStudio for Performance Marketing.

La siguiente tabla muestra los permisos predeterminados del administrador del sistema de GenStudio for Performance Marketing:

| Funcionalidad | Crear | Actualizar | Eliminar | Ver |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | yes | yes | yes | yes |
| [!DNL Campaigns] | yes | yes | yes | yes |
| [!DNL Content] | yes | yes | yes | yes |
| [!DNL Insights] | yes | yes | yes | yes |
| [!DNL Personas] | yes | yes | yes | yes |
| [!DNL Products] | yes | yes | yes | yes |
| [!DNL Reviews and approvals] | yes | yes | yes | yes |


## Preparación de GenStudio for Performance Marketing para generar contenido

Los administradores del sistema de GenStudio for Performance Marketing preparan el entorno de GenStudio for Performance Marketing de su organización para que los editores y colaboradores creen recursos de campaña. Estas tareas preliminares de configuración incluyen:

1. [Agregar directrices](./guidelines/overview.md) para [!DNL Brands], [!DNL Products] y [!DNL Personas]. La configuración de los componentes clave de la identidad de marca de su organización es un requisito previo esencial para el trabajo de los creadores y colaboradores. Puede cargar documentos de directrices de marca o introducir manualmente información de marca.
   * **Prepare sus documentos de directrices**. Cuanto más descriptivas y completas sean las directrices de marca, mejor será el resultado. Incluya ejemplos breves de las funciones que considera esenciales para su marca y agregue descripciones del comportamiento que desea excluir de la creación de contenido. GenStudio for Performance Marketing extrae información de estos documentos cargados y comienza a crear su marca. La información, como las directrices de voz, canal e imagen de la marca, se rellenan a medida que GenStudio for Performance Marketing organiza cada directriz a partir de los documentos cargados.
   * **Edite o complete los campos de las directrices de marca según sea necesario**. Las directrices de marca completas forman la base de la comprensión por parte de GenStudio for Performance Marketing de la marca de su organización. Una vez que GenStudio for Performance Marketing ha extraído la información que necesita de los documentos de directrices de marca, se le pedirá que edite o complete manualmente los campos de información extraída. Especifique áreas de enfoque de producto individuales para la creación de contenido agregando [!DNL Product]. Las directrices de [!DNL Personas] ayudan a adaptar la creación de contenido para segmentos de clientes definidos.

   Aunque la configuración de las directrices de marca de una organización puede ser una acción única, es posible que tenga que revisar y mejorar estas directrices en función de la volatilidad, el crecimiento y las circunstancias cambiantes del mercado de su organización.

1. **[Cargar plantillas](./content/use-templates.md)**. Las plantillas proporcionan métodos abreviados de teclado y aceleran la creación de contenido. Una plantilla contiene funciones aprobadas, como encabezados y pies de página, y establece protecciones para la creación de contenido. Normalmente, los administradores de sistemas cargan y administran plantillas para su organización. Los creadores utilizan plantillas para impulsar el proceso de creación de contenido dentro de los límites establecidos de la marca de la organización.

1. **[Cargar recursos aprobados](./content/manage-assets.md)**. Los recursos aprobados en [!DNL Content] están disponibles para todos los creadores de GenStudio for Performance Marketing. Puede inicializar [!DNL Content] con recursos que los creadores pueden usar para crear experiencias o recursos nuevos.

1. **[Conectarse a una cuenta de Meta (Facebook)](./insights/connect-channel.md)**. Configure una conexión entre GenStudio for Performance Marketing y las cuentas sociales de su organización para recibir datos de sus campañas de marketing, recursos y experiencias activos. [[!DNL Insights]](./insights/overview.md) proporciona herramientas para analizar datos derivados del canal.
