---
title: Prácticas recomendadas para plantillas
description: Siga las prácticas recomendadas al utilizar plantillas con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Prácticas recomendadas para usar plantillas

Las plantillas reducen significativamente el tiempo y el esfuerzo necesarios para generar contenido nuevo al proporcionar un punto de partida que incluye diseños y elementos de diseño preconfigurados.

Utilice las siguientes recomendaciones cuando utilice plantillas con GenStudio for Performance Marketing:

1. Obtenga información sobre [elementos de plantilla](#know-about-template-elements)
1. Configure [directrices de canal](#configure-channel-guidelines) para una personalización efectiva del contenido
1. Diseñe con [estándares de accesibilidad](accessibility-for-templates.md) para obtener una experiencia óptima
1. Seguir [directrices de plantillas específicas de canal](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>Obtenga más información acerca de los elementos y procedimientos básicos de la plantilla en [Trabajar con plantillas](use-templates.md). Y profundiza en [la personalización de una plantilla](customize-template.md) para usarla en tu próxima campaña.

## Información sobre los elementos de plantilla

Como práctica recomendada, familiarícese con las partes de una plantilla. Cada tipo de plantilla utiliza diferentes elementos para crear una estructura para la creación de contenido específica del canal. Para personalizar la plantilla, utilice los nombres de campo en lugar de estos elementos donde necesite que GenStudio for Performance Marketing genere contenido.

Ver [elementos de plantilla](use-templates.md#template-elements).

## Configuración de directrices de canal

Definir directrices de canal claras es esencial para garantizar que el contenido generado se ajuste a los requisitos y objetivos de la marca. Las directrices de canal permiten especificar reglas para elementos como el tono, la longitud y el estilo que se utilizan en la plantilla. Por ejemplo, puede establecer un recuento máximo de caracteres para el cuerpo o requerir un estilo call-to-action específico. Al establecer estas directrices por adelantado, reduce la necesidad de escribir instrucciones detalladas en cada mensaje de IA, lo que optimiza el proceso de generación de contenido y garantiza la coherencia en los correos electrónicos.

Revise y defina las [directrices de canal](/help/user-guide/guidelines/brands.md#channel-guidelines) de su marca para todos los campos clave de su plantilla. Si no define directrices, se aplican las [directrices predeterminadas para canales](/help/user-guide/guidelines/brands.md#default-channel-guidelines), que pueden no reflejar completamente los requisitos de su marca.

![Especificaciones del cuerpo](/help/assets/channel-email-body.png)

Conozca de qué manera las [directrices de marcas, productos y personas](/help/user-guide/guidelines/overview.md) influyen en el contenido generado y cómo adaptarlo a sus objetivos de marketing.

## Siga las directrices de plantillas específicas del canal

Al crear plantillas, asegúrese de que cumplen los requisitos específicos del canal al que va dirigido. Cree plantillas que se adapten al diseño y a los requisitos visuales de cada canal. Existen directrices generales que se aplican a cualquier plantilla, como:

- Utilizar HTML y CSS en línea limpios y adaptables
- Usar fuentes Adobe o Google
- **no** usa JavaScript

{{note-css-effects}}

Consulte más sugerencias y restricciones al trabajar con cada tipo de plantilla para garantizar un rendimiento óptimo:

- [Correos electrónicos](/help/user-guide/templates/email-template.md)
- [Publicidad en pantalla y banner](/help/user-guide/templates/display-template.md)
- [LinkedIn](/help/user-guide/templates/linkedin-template.md)
- [Anuncios de Meta](/help/user-guide/templates/meta-template.md)
