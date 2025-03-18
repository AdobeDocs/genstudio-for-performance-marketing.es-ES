---
title: Preparación de una plantilla de Meta ad para Adobe GenStudio for Performance Marketing
description: Aprenda a crear una plantilla de anuncio Meta personalizada para Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Media Templates
hidefromtoc: true
recommendations: noCatalog
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
source-git-commit: 19d0b8b929e293179a091cc7b5a6a1268b0abbbd
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Preparación de una plantilla de MetaAd para Adobe GenStudio for Performance Marketing

La creación de una plantilla de Meta ad implica un enfoque estructurado adaptado a los medios sociales. Después de diseñar y probar una plantilla de anuncio Meta, puede prepararla para su carga y uso en GenStudio for Performance Marketing.

## Adición de directrices

Antes de preparar una plantilla de anuncio Meta, asegúrese de haber agregado [directrices](/help/user-guide/guidelines/overview.md) a su GenStudio for Performance Marketing y de haberlas rellenado con información exhaustiva de las marcas relevantes. Las [directrices de marca](/help/user-guide/guidelines/brands.md) influyen directamente en el contenido generado.

**Ejemplo**: Si desea que el cuerpo de una plantilla de Meta ad no tenga más de 500 caracteres, agregue ese requisito a las [directrices de canal](/help/user-guide/guidelines/brands.md#channel-guidelines) para el campo &quot;cuerpo&quot;.

Si no se añaden directrices a GenStudio for Performance Marketing, se utilizan valores predeterminados.

## Diseño de una plantilla

Normalmente, un diseñador crea el diseño visual de una plantilla en un programa de diseño como Adobe XD.

Vea [Elementos de plantilla](use-templates.md#template-elements) y [Ejemplos de plantilla](/help/user-guide/content/customize-template.md#template-examples).

### Especificaciones del anuncio

GenStudio for Performance Marketing admite estas relaciones de aspecto para los anuncios Meta:

* Cuadrado (1:1): 1080 x 1080 píxeles
* Vertical (4:5): 1080 x 1350 píxeles
* Historia (9:16): 1080 x 1920 píxeles

Si el anuncio no está diseñado en ninguna de estas relaciones de aspecto, GenStudio for Performance Marketing recorta automáticamente la imagen en el tamaño adecuado.

## Prueba de una plantilla de publicidad Meta

Pruebe la plantilla con el Creative Hub de Meta para ver el aspecto del anuncio en diferentes ubicaciones, como en una fuente o como una historia.

Utilice la plataforma de envío o prueba de correo electrónico para probar el correo electrónico y comprobar que se procesa correctamente en diferentes clientes y dispositivos de correo electrónico.

## Definir áreas de contenido generadas

Defina las áreas en la plantilla de correo electrónico que deben rellenarse dinámicamente con contenido de GenStudio for Performance Marketing.

Para definir áreas de contenido generadas:

* Identifique los elementos de texto de la plantilla que GenStudio for Performance Marketing debe generar automáticamente, como el titular o CTA.
* Adapte la plantilla de HTML insertando marcadores de posición dentro de ella mediante la sintaxis Handlebars.

Consulte [Marcadores de posición de contenido](/help/user-guide/content/customize-template.md#content-placeholders).

## Previsualización de la plantilla

Controle la visibilidad de áreas de contenido específicas con los ayudantes integrados. Por ejemplo, incluya parámetros de seguimiento en los vínculos de una plantilla exportada mientras mantiene los vínculos de vista previa limpios.

Ver [vista previa de plantilla](/help/user-guide/content/customize-template.md#template-preview).

## Cargar y utilizar plantilla

Una vez diseñada, codificada, probada y previsualizada la plantilla, cárguela en GenStudio for Performance Marketing para utilizarla en la generación de contenido de marketing completamente nuevo.

Consulte [Uso de plantillas](use-templates.md).
