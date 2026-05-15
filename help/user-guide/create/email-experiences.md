---
title: Experiencias de correo electrónico
description: Obtenga información acerca de las experiencias de correo electrónico en Adobe GenStudio for Performance Marketing, incluido el comportamiento del lienzo y el intercambio de fragmentos de contenido de bibliotecas aprobadas.
feature: Create Canvas, Media Templates
role: User
level: Beginner
exl-id: e2bddd02-914e-43a8-92b6-fdcbced94a6a
TQID: https://experienceleague.adobe.com/-lwSfvc0TnVd8byNT-5OfoEsXz7yaeIifcHOJtp-n4c
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2:
  - id: a8b28c00-da6e-4d27-8667-80f790ad8972
  - id: be495d08-ecd1-455f-951e-c22de504e667
  - id: dee4e9a9-78d1-4953-8179-f8da6117027d
  - id: ee4b6e5f-5b7a-421b-9859-0f964841a866
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: e41ca23a135e2cacfcc029c04992bbff1b515bd6
workflow-type: tm+mt
source-wordcount: 580
ht-degree: 0%

---

# Experiencias de correo electrónico

Con Adobe GenStudio for Performance Marketing, puedes usar IA generativa para optimizar la [creación de experiencias de correo electrónico de alto impacto](/help/user-guide/create/create-email-experience.md).

[!DNL Create] permite que los especialistas en marketing moderno usen [directrices](/help/user-guide/guidelines/overview.md), recursos de imagen y un [mensaje bien diseñado](/help/user-guide/effective-prompts.md) para [crear rápidamente experiencias de correo electrónico alineadas con la marca](/help/user-guide/create/create-email-experience.md).

Al generar experiencias por correo electrónico, se crean cuatro variaciones que se muestran en el lienzo.

Las secciones editables de una experiencia de correo electrónico incluyen:

* Pre-encabezado
* Titular
* Subtítulo
* Cuerpo
* Call to action (CTA)
* Imagen

Ver [elementos de plantilla](/help/user-guide/templates/use-templates.md#template-elements).

<!-- 
## Email capabilities

Content creators and marketers can produce brand-consistent email experiences in GenStudio for Performance Marketing. 
-->

## Correos electrónicos de varias secciones

Las experiencias de correo electrónico pueden tener varias secciones, lo que permite una personalización completa para alinearse con la marca y los objetivos. [Seleccione [!DNL Products] y recursos visuales para cada sección](/help/user-guide/create/create-email-experience.md#add-parameters) y use [mensajes estructurados](/help/user-guide/effective-prompts.md#structured-prompts) para crear contenido único. Cada sección admite un recurso visual.

Consulte [personalización de plantillas con secciones](/help/user-guide/templates/customize-template.md#sections-or-groups) para obtener información sobre cómo crear una plantilla de varias secciones.

## Carga progresiva

Cuando se inicia el proceso de generación de contenido, cada sección del contenido generado en las variantes de correo electrónico se carga progresivamente en el lienzo. Las experiencias, los recursos, los campos y las secciones dentro de las experiencias aparecen individualmente en el lienzo a medida que se generan.

Al hacer clic en **[!UICONTROL Generar]**, aparece un indicador de carga en la parte inferior del lienzo que le actualiza en el progreso de generación.

Cada campo y sección de experiencias de correo electrónico se cargan progresivamente en esta secuencia:

1. Nombres de variante
1. Líneas de asunto para todas las variaciones
1. Encabezados previos
1. Titulares, cuerpo del correo electrónico (para correos electrónicos de una sola sección) y llamadas a la acción
1. Cuerpo del correo electrónico para las secciones siguientes (para correos electrónicos de varias secciones)
1. Validación de marca

   Se lleva a cabo el proceso de validación de marca y comprobación de contenido y el [_resumen de la comprobación de contenido_](/help/user-guide/guidelines/brand-validation.md#content-check-summary) se rellena para cada variante.

## Recuentos de caracteres

Después de generar un conjunto de variantes de correo electrónico, puede ver el recuento de caracteres que se muestra para cada sección. Pase el ratón sobre una sección generada (por ejemplo, la línea de asunto o el cuerpo) o haga clic en ella y vea el nombre de la sección y el recuento de caracteres de dicha sección.

![Recuento de caracteres](/help/assets/character-count.png){width="500" zoomable="yes"}

## Intercambio de fragmentos de contenido {#content-fragment-swap}

>[!NOTE]
>
>El intercambio de fragmentos de contenido está disponible para las experiencias de **correo electrónico** en el lienzo hoy. La compatibilidad con el canal **Horizon** estará disponible próximamente.

El contenido del correo electrónico empresarial a menudo necesita bloques modulares recién generados y aprobados (como exenciones de responsabilidad, lenguaje de seguridad, ofertas y reclamaciones reguladas) junto con el contenido que forma para las plantillas. Los equipos que almacenan contenido modular en [!DNL Adobe Experience Manager] pueden buscar e intercambiar ese contenido para utilizarlo en las experiencias de correo electrónico sin salir de [!DNL GenStudio for Performance Marketing]. Esto puede resultar útil para lo siguiente:

* **Contenido con reconocimiento de cumplimiento:** IA puede llenar espacios creativos mientras que los fragmentos aprobados por el cumplimiento reemplazan los espacios inyectables; las áreas legales bloqueadas permanecen sin cambios a través de la exportación.
* **Componentes de contenido aprobado reutilizables:** Los titulares aprobados, las exenciones de responsabilidad regional o las descripciones de productos pueden seguir siendo el sistema de registro en [!DNL Adobe Experience Manager] mientras los autores los extraen en variantes sin tener que copiar y pegar soluciones alternativas.

Los creadores reúnen las experiencias en el lienzo; los equipos de conformidad y marca mantienen los flujos de trabajo de aprobación en [!DNL Adobe Experience Manager]; los equipos de TI e integraciones conectan repositorios y permisos que requiere su organización.

![Intercambio de fragmento de contenido](./cf-swap.png){width="500" zoomable="yes"}

Cuando su organización habilita el intercambio de fragmentos de contenido, puede esperar lo siguiente:

* Los campos de fragmento de contenido se pueden rellenar desde una biblioteca de contenido conectada en lugar de solo escribir manualmente o generar IA.
* Examine, busque y filtre fragmentos con metadatos como campaña, perfil, canal, idioma y marca.
* Un selector de repositorios está disponible cuando hay varios repositorios configurados.
* Vista previa de un fragmento antes de reemplazar el texto del campo.
* Propagación de una selección de fragmentos en todas las variantes en una acción.

![Panel de IU de fragmentos de contenido](./cf-pane.png){width="500" zoomable="yes"}

Su organización elige qué fuentes de fragmentos de contenido y repositorios están disponibles. Consulte [Buscar extensión de fragmento de contenido](/help/extensibility/deploy-app.md#find-content-fragment-extension) para ver cómo configuran los administradores las fuentes y cómo los autores intercambian la copia del lienzo con **[!UICONTROL Intercambiar]**.
