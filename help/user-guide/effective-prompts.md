---
title: Escribir indicadores efectivos
description: Aprenda a escribir mensajes efectivos para Adobe GenStudio for Performance Marketing.
feature: Prompt, Generative AI, Brands Service, Personas Service, Products Service, Guidelines
exl-id: 0cd4db4f-d031-4c1f-a4e7-adc220f947fc
source-git-commit: 449c212ab167a6c126492e9becedf9318bfe08ee
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# Escribir indicadores efectivos

La comunicación con la IA generativa es esencial para trabajar de forma eficaz en Adobe GenStudio for Performance Marketing.

GenStudio for Performance Marketing proporciona un aviso de IA generativo cada vez que se ofrece la oportunidad de modificar un recurso. Los componentes de un mensaje eficaz deben incluir lenguaje descriptivo, ejemplos e información que no se proporciona a través de las directrices configuradas.

Como práctica recomendada, proporcione a GenStudio for Performance Marketing su información de marca mediante [directrices](/help/user-guide/guidelines/overview.md) para que pueda aprovechar al máximo la IA generativa a fin de producir experiencias de contenido alineadas con la marca.

## Lenguaje descriptivo

Puede utilizar el lenguaje natural para articular sus ideas y crear experiencias. El mensaje guía la IA para generar contenido de canal personalizado e imágenes que complementen su visión. Cuantos más detalles proporcione, mayores serán las posibilidades de producir una imagen o una experiencia que satisfaga sus necesidades. Utilice un lenguaje claro y descriptivo para proporcionar tantos detalles como sea posible:

- Para **imágenes**, usa palabras que describan ambiente, humor, color, composición y estilo.
- Para **copiar**, usa palabras que describan la audiencia, el propósito, las nuevas descripciones de características, los ejemplos y las acciones.

A continuación se muestra un ejemplo de mensaje que articula información sobre la intención, la audiencia de destino y el estilo.

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.
```

+++Ver resultados de ejemplo

![tres correos electrónicos generados](/help/assets/sample-email.png)

+++

## Criterios de solicitud

En GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md), puede usar **[!UICONTROL Criterios del indicador]** ([_Parámetros_](/help/user-guide/create/overview.md#parameters) y un indicador) en el cajón del indicador para agregar detalles a través de la selección y mejorar la interpretación de IA.

Para [correos electrónicos](/help/user-guide/create/email-experiences.md), los criterios de solicitud pueden incluir la adición de [directrices](/help/user-guide/guidelines/overview.md) en _Parámetros_, la carga de un recurso para utilizarlo en las variantes de correo electrónico y una solicitud descriptiva. Para un [Meta ad](/help/user-guide/create/create-meta-ad.md), los criterios de solicitud pueden incluir una directriz de marca en _Parámetros_, la selección o carga de un recurso existente, la configuración relacionada con imágenes o recursos como la proporción de aspecto y un mensaje. El poder real comienza con [configurar directrices](/help/user-guide/guidelines/add-guidelines.md).

>[!NOTE]
>
>Si se agregan directrices en _Parameters_ en el cajón de mensajes, no es necesario incluir una referencia a ellas en el mensaje. GenStudio for Performance Marketing aprovecha [!DNL Brands], [!DNL Products] y [!DNL Personas] en la generación de contenido.

### Directrices

Las directrices de GenStudio for Performance Marketing ayudan a la IA generativa a personalizar la composición de los recursos. Cuando se le presenten criterios de solicitud, puede elegir un [[!DNL Brand]](/help/user-guide/guidelines/brands.md), un [[!DNL Persona]](/help/user-guide/guidelines/personas.md) y un [[!DNL Product]](/help/user-guide/guidelines/products.md) de entre las directrices configuradas.

>[!TIP]
>
>Usted controla cómo y cuándo GenStudio for Performance Marketing usa sus directrices de [!DNL Brand]. Consulte [Directrices](/help/user-guide/guidelines/overview.md) para obtener información sobre cómo configurar y administrar las directrices de marca.

### Indicadores estructurados

En el caso de los correos electrónicos de varias secciones, puede estructurar las solicitudes para proporcionar instrucciones específicas de cada sección a fin de generar contenido variable para cada sección en un [correo electrónico](/help/user-guide/create/email-experiences.md). Los mensajes estructurados deben hacer referencia directamente a [nombres de sección en la plantilla de correo electrónico](/help/user-guide/content/email-template.md#multi-section-emails) para que el contenido generado se pueda insertar en los marcadores de posición de contenido correspondientes.

Por ejemplo, puede indicar a GenStudio for Performance Marketing que genere contenido que promocione un nuevo producto en la primera sección de un correo electrónico y que genere contenido que detalle las ventajas de ahorro del producto en la segunda sección de correo electrónico.

La petición de datos estructurada debería:

- Utilice una de las siguientes referencias al nombre de sección en la plantilla de correo electrónico:
   - Pod
   - Grupo
   - Sección
   - Módulo

  Por ejemplo, si la plantilla usa `moduleA` o `Group-3` como nombre de sección, puede hacer referencia a esos nombres de sección en el mensaje.

- Siga las reglas o la estructura recomendadas. Si la estructura de la solicitud no cumple el formato proporcionado, se aplica a *todas* las secciones de correo electrónico y sigue facilitando la generación de contenido.
- Use nombres de sección como [definidos en su plantilla de correo electrónico](/help/user-guide/content/email-template.md#code-an-email-template). Las referencias de solicitud deben coincidir con los nombres de sección codificados en la plantilla de correo electrónico.
- No distinguir mayúsculas de minúsculas. Por ejemplo, puede usar `Pod` o `pod` en la plantilla de correo electrónico y en la solicitud estructurada.
- Consulte primero el símbolo del sistema genérico y, a continuación, las directivas específicas de sección.
- Use dos puntos, un guión, una coma u otra demarcación (`,:;#$!~|@=-%&*^_`) como separación entre la referencia del nombre de sección y la directiva. Por ejemplo, puede usar lo siguiente como directiva de solicitud específica de la sección: `Pod1; Describe how to easily edit text and swap images.`

El siguiente es un ejemplo de mensaje que articula la estructura de mensajes recomendada y aprovecha una plantilla de correo electrónico que utiliza el término de identificación `Pod` como en `Pod1`, `Pod2` y `Pod3`.

```properties
Create an exciting multi-pod email focusing on Creative Cloud and its powerful generative AI capabilities.

Encourage customers to convert to Photoshop or use a free Photoshop trial. We want to better educate them about app features.

Pod1: Focus on Adobe Photoshop and its new generative AI tools that enable creators to bring images to life in minutes.

Pod2: Focus on Adobe Illustrator and its new generative AI tools, such as Generative Shape Fill, which allows you to quickly fill your vector outline and explore a variety of options that match the look and feel of your own artwork.

Pod3: Focus on Adobe Acrobat Pro. Make users aware that with Acrobat Pro they can edit images and text inside a PDF.
```

Consulte [Preparar una plantilla de correo electrónico](/help/user-guide/content/email-template.md#code-an-email-template).

## Inténtelo de nuevo

La solicitud es un proceso iterativo. Si los resultados no cumplen con sus expectativas, revise el mensaje y realice algunos cambios o agregue más detalles. O bien, puede pegar en secciones de un informe de campaña. Incluso puede solicitar que GenStudio for Performance Marketing evite determinadas palabras, elementos o temáticas.

## Prácticas recomendadas

Algunas prácticas recomendadas sencillas para crear indicadores eficaces:

- Sea específico y proporcione detalles sobre qué hacer y qué no hacer.
- Proporcionar contexto mediante referencias externas.
- Aproveche las directrices de GenStudio for Performance Marketing.
- Revise y ajuste las directrices regularmente.
- Iterar y refinar.
- Aprenda con la experimentación.
