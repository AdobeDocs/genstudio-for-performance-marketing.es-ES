---
title: Preparar una plantilla de correo electrónico para Adobe GenStudio for Performance Marketing
description: Obtenga información sobre cómo crear una plantilla de correo electrónico personalizada para Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Media Templates
hidefromtoc: true
recommendations: noCatalog
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: 19d0b8b929e293179a091cc7b5a6a1268b0abbbd
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Preparar plantilla de correo electrónico para Adobe GenStudio for Performance Marketing

Normalmente, un diseñador crea el diseño visual de una plantilla en un programa de diseño como Adobe XD. Una vez diseñada, codificada y probada una plantilla de correo electrónico, puede prepararla para su carga y uso en GenStudio for Performance Marketing.

Ver [elementos de plantilla](use-templates.md#template-elements).

## Adición de directrices

Antes de preparar una plantilla de anuncio Meta, asegúrese de haber agregado [directrices](/help/user-guide/guidelines/overview.md) a su GenStudio for Performance Marketing y de haberlas rellenado con información exhaustiva de las marcas relevantes. Las [directrices de marca](/help/user-guide/guidelines/brands.md) influyen directamente en el contenido generado.

**Ejemplo**: Si desea que el cuerpo de una plantilla de correo electrónico no tenga más de 500 caracteres, agregue ese requisito a las [directrices de canal](/help/user-guide/guidelines/brands.md#channel-guidelines) para el campo &quot;cuerpo&quot;.

Si no se añaden directrices a GenStudio for Performance Marketing, se utilizan valores predeterminados.

## Codifique una plantilla de correo electrónico

Una vez diseñada una plantilla, se codifica con HTML y CSS en línea. El código debe ser limpio y adaptable para varios dispositivos.

Ver [ejemplos de plantillas](/help/user-guide/content/customize-template.md#template-examples).

### Correos electrónicos de varias secciones

Puede usar [mensajes estructurados](/help/user-guide/effective-prompts.md#structured-prompts) durante la generación de contenido para indicar a GenStudio for Performance Marketing que genere contenido variable por sección de un correo electrónico.

Por ejemplo, si las secciones de la plantilla de correo electrónico tienen el prefijo `Pod`—`Pod1` y `Pod2`, la solicitud estructurada para la generación de contenido puede incluir directivas específicas para esas secciones de correo electrónico. GenStudio for Performance Marketing hace coincidir la directiva específica de la sección del mensaje con la sección de correo electrónico relacionada y genera contenido alineado con las directivas.

Consulte [Mensajes estructurados](/help/user-guide/effective-prompts.md#structured-prompts).

## Prueba de una plantilla de correo electrónico

Utilice la plataforma de envío o prueba de correo electrónico para probar el correo electrónico y comprobar que se procesa correctamente en diferentes clientes y dispositivos de correo electrónico.

Pruebe para asegurarse de que la plantilla de correo electrónico cumple lo siguiente:

* El diseño se ajusta para diferentes tamaños de pantalla mediante consultas de medios CSS
* Se puede hacer clic en los botones y desplazarse hasta el lugar deseado
* La plantilla de correo electrónico se puede leer y utilizar en dispositivos móviles

## Definir áreas de contenido generadas

Defina las áreas en la plantilla de correo electrónico que deben rellenarse dinámicamente con contenido de GenStudio for Performance Marketing.

Para definir áreas de contenido generadas:

* Identifique los elementos de texto de la plantilla que GenStudio for Performance Marketing debe generar automáticamente, como el titular o CTA.
* Adapte la plantilla de HTML insertando marcadores de posición dentro de ella mediante la sintaxis Handlebars.

Consulte [Marcadores de posición de contenido](/help/user-guide/content/customize-template.md#content-placeholders).

## Previsualización de la plantilla

Controle la visibilidad de áreas de contenido específicas con los ayudantes integrados. Por ejemplo, puede incluir parámetros de seguimiento en vínculos en una plantilla exportada mientras mantiene los vínculos de vista previa limpios.

Ver [vista previa de plantilla](/help/user-guide/content/customize-template.md#template-preview).

## Cargar y utilizar plantilla

Una vez diseñada, codificada, probada y previsualizada la plantilla, puede cargarla en GenStudio for Performance Marketing para utilizarla en la generación de contenido de marketing completamente nuevo.

Consulte [Uso de plantillas](use-templates.md).
