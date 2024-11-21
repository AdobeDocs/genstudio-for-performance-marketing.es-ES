---
title: Introducción a Adobe GenStudio for Performance Marketing
description: Aprenda a configurar su GenStudio para Performance Marketing para generar nuevo contenido de marketing alineado con la marca.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: bcb03198-bbcb-45ae-af01-25c1e834b563
source-git-commit: 3c391753ebd0d19ad7dcb17870915eeccc55cc05
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 2%

---

# Introducción a Adobe GenStudio for Performance Marketing

Adobe GenStudio for Performance Marketing ofrece un completo conjunto de herramientas diseñadas para optimizar la creación, administración y análisis de contenido. Infunde al ciclo vital de creación de contenido funciones de IA generativas que transforman la forma en que se crea, revisa, comparte y analiza el contenido de marketing.

## Empezar a crear, compartir y revisar contenido

Si no tiene experiencia previa con herramientas generativas basadas en IA o simplemente siente curiosidad por conocer los principios básicos de GenStudio for Performance Marketing, consulte [Conceptos](concepts.md) y [Escribir mensajes efectivos](effective-prompts.md). Puedes consultar la [Academia de Adobe GenStudio](https://learningmanager.adobe.com/genstudioacademy), la plataforma de aprendizaje en línea de Adobe, sobre el uso de tecnologías de IA generativa en el proceso creativo.

## Entrenar GenStudio for Performance Marketing

GenStudio for Performance Marketing utiliza información sobre su marca y sus mercados para mejorar la creación de contenido compatible con la marca. Los materiales de capacitación incluyen ejemplos, descripciones de [personalidades](/help/user-guide/guidelines/personas.md) y [productos](/help/user-guide/guidelines/products.md) del cliente, y [directrices de marca](/help/user-guide/guidelines/overview.md).

Los administradores de sistemas configuran Adobe GenStudio for Performance Marketing introduciendo o cargando información específica de la organización. Esta preparación garantiza que los editores de contenido y los colaboradores puedan utilizar de forma eficaz las funciones de IA generativa para crear y revisar recursos de la campaña. Una vez que un administrador del sistema de Adobe aprovisiona la instancia de producto de su organización y asigna permisos de administrador del sistema de GenStudio, el administrador del sistema de GenStudio puede preparar la estructura de IA generativa subyacente del producto mediante directrices.

### Paso 1: Añadir directrices

La configuración de los componentes clave de la identidad de marca de su organización es un requisito previo esencial para el trabajo de los editores de contenido y los colaboradores. [Directrices](./guidelines/overview.md) capturan características de la marca, como logotipos, tono de voz y paletas de color. Puede cargar documentos de [[!DNL Brands] guidelines](./guidelines/brands.md) o escribir manualmente la información de marca. [[!DNL Personas] directrices](./guidelines/personas.md) y [[!DNL Products] directrices](./guidelines/products.md) también son importantes. Las capacidades generativas de IA subyacentes de GenStudio for Performance Marketing utilizan estas directrices para establecer protecciones que guíen la generación de contenido.

#### Preparación de los documentos de directrices

Las directrices detalladas y centradas de [[!DNL Brands]](./guidelines/brands.md), [[!DNL Products]](./guidelines/products.md) y [[!DNL Personas]](./guidelines/personas.md) definen aspectos básicos de las campañas de marketing de su organización. GenStudio for Performance Marketing extrae información de estas directrices para empezar a crear su marca.

Siga estas prácticas recomendadas al preparar las directrices:

* Utilice un idioma específico.

* Incluya los mejores ejemplos que pueda encontrar del estilo y el tono que desea que incorporen los recursos de la campaña.

* Evite la redundancia. Puede sentirse tentado a repetir una directiva varias veces, pero la redundancia en sus directrices no ayuda al LLM subyacente a capturar e implementar sus directrices de marca.

* Identifique los elementos que desea que el LLM excluya durante la generación de contenido (por ejemplo, exclamaciones en el texto).

Puede cargar documentos de directrices o consultarlos cuando introduzca manualmente información en GenStudio for Performance Marketing. Consulte [Agregar directrices](./guidelines/overview.md) para obtener instrucciones sobre cómo cargar o escribir esta información.

#### Revisar directrices

Un administrador del sistema de GenStudio puede preparar la estructura de IA generativa subyacente del producto introduciendo o cargando manualmente los requisitos de marca específicos de su organización. Aunque la configuración de las directrices de marca de una organización es una acción única, puede revisar y mejorar estas directrices en función de la volatilidad, el crecimiento y las circunstancias cambiantes del mercado de su organización.

## Paso 2: Configurar un proyecto de Adobe Admin Console para GenStudio [!DNL Brands]

Los administradores del sistema deben completar tareas de configuración adicionales para que los colaboradores puedan editar o crear [!DNL Brands]. Los administradores del sistema de Adobe realizan estas tareas en Adobe Admin Console:

* Cree un nuevo grupo de usuarios que incluya a todos los usuarios que necesitan editar y crear [!DNL Brands] autorizaciones.

* Cree un nuevo proyecto en Adobe Admin Console.

Consulte [Asignar permisos de marca](configure-brand-permissions.md).

### Paso 3: Cargar plantillas

Las plantillas aceleran la creación de contenido. Una plantilla contiene funciones aprobadas, como encabezados y pies de página, y está optimizada para canales específicos. Normalmente, los administradores de sistemas cargan y administran plantillas para su organización. Los editores de contenido utilizan plantillas para impulsar el proceso de creación de contenido dentro de los límites establecidos de la marca de la organización.

Ver [Trabajar con plantillas](./content/use-templates.md).

### Paso 4: cargar los recursos aprobados

Los recursos aprobados en [!DNL Content] están disponibles para todos los editores de GenStudio for Performance Marketing. Puede rellenar [!DNL Content] con recursos que los editores de contenido pueden usar en la creación de experiencias o recursos nuevos.

Ver [Cargar recursos aprobados](./content/manage-assets.md).

### Paso 5: Conectarse a una cuenta de Meta (Facebook)

Configure una conexión entre GenStudio for Performance Marketing y las cuentas sociales de su organización para recibir datos de sus campañas de marketing, recursos y experiencias activos. [[!DNL Insights]](./insights/overview.md) proporciona herramientas para analizar datos derivados del canal. Ver [Conectarse a una cuenta de Meta (Facebook)](./insights/connect-channel.md#meta-ads-connect).
