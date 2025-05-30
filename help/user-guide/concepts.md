---
title: Conceptos de Adobe GenStudio for Performance Marketing
description: Aprenda los conceptos y la terminología de Adobe GenStudio for Performance Marketing.
feature: Generative AI
role: User
exl-id: 7dd00b4c-f429-499b-851d-3606c82c09dc
source-git-commit: 78313c2a2177a2ccb39e37a87ca3c657e7906d0a
workflow-type: tm+mt
source-wordcount: '699'
ht-degree: 0%

---

# Conceptos 

GenStudio for Performance Marketing es un producto empresarial independiente que encarna la cadena de suministro de contenido de Adobe para optimizar las campañas de marketing. Es difícil crear contenido personalizado y aprobado por la marca a escala, monitorizar la eficacia y adaptarse rápidamente al mercado en constante cambio. GenStudio for Performance Marketing reúne a Creative Cloud y Experience Cloud en una aplicación que aprovecha la IA generativa como multiplicador de rendimiento para los equipos de marketing empresarial.

Con GenStudio for Performance Marketing puede:

* Cree contenido de marca mediante mensajes en lenguaje natural para sus canales digitales de máxima prioridad, como medios de pago, correo electrónico y anuncios en pantalla

* Colaboración con las partes interesadas para revisar y aprobar el contenido generado
* Guardar contenido generado y aprobado para acceder a él en futuras campañas de marketing
* Evalúe la eficacia del contenido analizando el rendimiento del recurso e identificando los atributos clave del contenido de mayor rendimiento

## Tecnología de IA generativa

GenStudio for Performance Marketing aprovecha el poder de la IA generativa para acelerar el proceso de creación de contenido y garantizar la generación de contenido de alta calidad. El ciclo de vida iterativo de los recursos creativos resulta en contenido cada vez más preciso y alineado con la marca que resuena con la audiencia de destino.

Comience por ingerir la marca, las personalidades del cliente y las descripciones de los productos de su organización a través de la potente función de directrices de marca. Consulte la [descripción general de las directrices](../user-guide/guidelines/overview.md) para obtener información sobre cómo preparar y cargar estas directrices.

{{in-academy}}

### Modelos de lenguaje grande

GenStudio for Performance Marketing aprovecha la plataforma de IA generativa de Adobe, que ofrece servicios fundamentales de IA y aprendizaje automático (ML). Esta plataforma simplifica el uso de modelos de lenguaje de gran tamaño (LLM), lo que permite que las capacidades GenAI de Adobe creen experiencias atractivas.

GenStudio for Performance Marketing usa la serie GPT de LLM de terceros a través de Azure OpenAI.<!-- Claude, and Gemini models. -->

## [!DNL Generative Actions]

_[!DNL Generative Actions]_, tal como se define en la [descripción del producto de Adobe GenStudio for Performance Marketing](https://helpx.adobe.com/es/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html), son las unidades que cuantifican el uso de características de IA generativa dentro de GenStudio for Performance Marketing.

<!-- Add example about usage mode?
Where users check how many generative actions they have left
How they re-up their genactions
If genactions roll over month to month or not -->

### Tarifas

Recibirá una asignación predeterminada de [!DNL Generative Actions] como se describe en la [descripción del producto de GenStudio for Performance Marketing](https://helpx.adobe.com/es/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html).

>[!NOTE]
>
>Las tasas de uso pueden variar. Los planes están sujetos a cambios. Consulte la [descripción del producto de Adobe GenStudio for Performance Marketing](https://helpx.adobe.com/es/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html) para obtener información actualizada sobre la tarifa.

Las siguientes funciones consumen [!DNL Generative Actions] a la velocidad especificada.

| Función | Tasa de acciones generativas |
| -----------------------  | ------------------ |
| Crear correo electrónico | 5 por generación |
| Creación de anuncios de medios pagados | 5 por generación |
| Creación de anuncios en pantalla | 5 por generación |
| Regenerar secciones | 1 por generación |

<!-- | Generate on-brand images | 1 per prompt  |
| Translation              | 1 per prompt  |
| Video: ADLS              | 1 per prompt  |
| Video: TTS + Avatar      | 1 per prompt  | -->

[!DNL Generative Actions] _no se_ consumen cuando:

* Usando [validación de marca](/help/user-guide/guidelines/brand-validation.md) durante la generación de variante
* Extrayendo información de [directrices cargadas](/help/user-guide/guidelines/add-guidelines.md)
* [Volver a comprobar las variantes](/help/user-guide/guidelines/brand-validation.md#improve-brand-alignment) manualmente
* Los recursos digitales se etiquetan automáticamente con atributos ([[!DNL Insights]](/help/user-guide/insights/overview.md))

>[!TIP]
>
>Si supera su asignación de [!DNL Generative Actions], puede comprar más directamente a su representante de cuentas.

## Gobernanza de datos

Al trabajar con IA para generar contenido, es esencial asegurarse de que el resultado sea seguro e inclusivo para todos los usuarios. Esto requiere la evaluación del contenido para detectar posibles sesgos dañinos, discursos de odio, material ofensivo o blasfemias. Adobe prueba exhaustivamente la tecnología de generación de contenido desde múltiples perspectivas, realiza revisiones éticas exhaustivas e implementa planes de mitigación eficaces para evitar que el contenido perjudicial aparezca en los resultados.

Este enfoque refuerza la responsabilidad social, minimiza el riesgo de reputación y garantiza el cumplimiento de las [políticas de Confianza y Seguridad y Ética de Adobe](https://www.adobe.com/content/dam/cc/en/ai-ethics/pdfs/Adobe-AI-Ethics-Principles.pdf).

GenStudio for Performance Marketing incorpora planes de mitigación para evitar el uso de contenido nocivo o sesgado identificado según las normas y políticas de gobernanza de datos de Adobe. Cuando se detecta dicho contenido, se le indica que la generación de recursos está bloqueada con el mensaje &quot;No se puede generar&quot;.

Cuando aparezca este mensaje, puede editar la solicitud e intentarlo de nuevo _o_ para marcar el contenido de la solicitud y que GenStudio for Performance Marketing lo revise. Los datos del mensaje para el contenido marcado para revisión se recopilan con fines de revisión interna.

## Ciclo de contenido

La demanda es alta para experiencias de calidad en varios canales a un ritmo más rápido. GenStudio for Performance Marketing simplifica la cadena de suministro de contenido para convertirla en un flujo de trabajo bien organizado para los especialistas en marketing. GenStudio for Performance Marketing aprovecha la tecnología de Adobe en cada fase del ciclo de vida.

<table style="table-layout:auto">

<tr style="border: 0;">

    <td>

       <p><strong>Flujo de trabajo y planificación</strong></p>

    </td>

    <td>

        <p>Haga una lluvia de ideas, defina directrices y cree una estrategia en torno al contenido para atraer a su audiencia.</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>Creación y producción</strong></p>

    </td>

    <td>

        <p>Produzca el contenido en función del plan. Colabore en tiempo real, reciba comentarios, realice ediciones y apruebe contenido.</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>Gestión de contenido</strong></p>

    </td>

    <td>

        <p>Almacene, comparta y busque recursos creativos en el repositorio centralizado. Reutilice y revitalice contenido en función del rendimiento.</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>Envío y activación</strong></p>

    </td>

    <td>

        <p>Active el contenido y publíquelo en varios canales de marketing.</P>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>Informes e información</strong></p>

    </td>

    <td>

        <p>Recopile datos y obtenga perspectivas para la optimización del rendimiento de los recursos.</p>

    </td>

</tr>

</table>
