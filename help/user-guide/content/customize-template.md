---
title: Personalizar una plantilla
description: Aprenda a personalizar y optimizar su plantilla para Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Templates, Content
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: 62ab3849296195ca4d9525cb5688f74ce8bede54
workflow-type: tm+mt
source-wordcount: '1281'
ht-degree: 0%

---

# Personalizar una plantilla

Puede personalizar una plantilla para utilizarla en GenStudio for Performance Marketing insertando marcadores de posición o campos de contenido que la API generativa utiliza para insertar contenido.

En las siguientes secciones se explica cómo adaptar las plantillas de HTML para GenStudio for Performance Marketing utilizando el idioma de plantilla _[!DNL Handlebars]_. La sintaxis [!DNL Handlebars] utiliza texto normal con llaves dobles como marcadores de posición de contenido. Consulte [Qué es [!DNL Handlebars]](https://handlebarsjs.com/guide/#what-is-handlebars) en la_ Guía de idioma de Handlebars _para aprender a preparar la plantilla.


Una vez que la plantilla esté lista, puedes [cargarla en GenStudio for Performance Marketing](use-templates.md#upload-a-template) y empezar a generar correos electrónicos personalizados basados en la plantilla personalizada.

>[!TIP]
>
>Siga las [directrices de accesibilidad](accessibility-for-templates.md) y las [prácticas recomendadas](/help/user-guide/content/best-practices-for-templates.md) para que pueda llegar a más audiencia y proporcionar una experiencia óptima.

## Marcadores de contenido

GenStudio for Performance Marketing reconoce ciertos [elementos](use-templates.md#template-elements) dentro de una plantilla, pero solo si los identifica con un nombre de campo reconocido.

Dentro del encabezado o del cuerpo de una plantilla, puede utilizar la sintaxis [!DNL Handlebars] como marcador de posición de contenido donde necesita que GenStudio for Performance Marketing rellene la plantilla con contenido real. GenStudio for Performance Marketing reconoce e interpreta los marcadores de posición de contenido en función del [nombre de _campo_ reconocido](#recognized-field-names).

Por ejemplo, puede usar `{{ headline }}` con la sintaxis [!DNL Handlebars] para indicar dónde se debe colocar el titular del correo electrónico:

```handlebars
<div>{{headline}}</div>
```

### Nombres de campo reconocidos

En la tabla siguiente se enumeran los nombres de campo reconocidos por GenStudio for Performance Marketing para la población en plantillas. Agregue estos nombres de campo con la sintaxis [!DNL Handlebars] a la plantilla donde necesite que GenStudio for Performance Marketing genere contenido.

| Campo | Función | Plantilla de canal |
| ------------------ | ---------------------- | -------------------------------- |
| `{{pre_header}}` | Encabezado previo | email |
| `{{headline}}` | Titular | correo electrónico <br>Meta ad <br>anuncio de visualización |
| `{{body}}` | Copia de cuerpo | correo electrónico <br>Meta ad <br>anuncio de visualización |
| `{{cta}}` | Llamada a la acción | correo electrónico <br>Meta ad <br>anuncio de visualización |
| `{{on_image_text}}` | En texto de imagen | Meta anuncio |
| `{{image}}` | Imagen: seleccionar del contenido | correo electrónico <br>Meta ad <br>anuncio de visualización |
| `{{brand_logo}}` | Logotipo de la marca seleccionada<br>Consulte [Nombre del campo del logotipo de la marca](#brand-logo-field-name) para ver el uso recomendado. | correo electrónico<br>Meta anuncio |

GenStudio for Performance Marketing rellena ciertos campos automáticamente en las siguientes plantillas:

- **La plantilla de correo electrónico** no requiere que identifique el campo `subject`
- **La plantilla de anuncios Meta** no requiere que identifique los campos `headline`, `body` y `CTA`
- **La plantilla de anuncios de visualización** no requiere que identifique el campo `CTA`

>[!WARNING]
>
>En el caso de los anuncios de Instagram, el titular generado no aparece en la experiencia final.

Hay un límite de 20 campos al cargar una plantilla en GenStudio for Performance Marketing. Dado que el campo `subject` se genera automáticamente en un mensaje de correo electrónico, se cuenta como un campo. Esto significa que hay 19 campos permitidos en una plantilla de correo electrónico.

>[!TIP]
>
>Puede comprobar su plantilla con la [vista previa de la plantilla](#template-preview) en GenStudio for Performance Marketing.

#### Nombre del campo del logotipo de marca

En este momento, no puede seleccionar el logotipo de la marca para cargar la plantilla. Los siguientes ejemplos muestran dos métodos que representan de forma condicional el logotipo de la marca. Cada método verifica el origen, proporciona una imagen predeterminada o alternativa en caso de que el logotipo de la marca no esté disponible y aplica un estilo:

**Ejemplo 1**: Se usa la condición [!DNL Handlebars] de los ayudantes integrados directamente en el atributo del HTML `img src`:

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Ejemplo 2**: Se usa [!DNL Handlebars] instrucción de condición integrada para envolver la etiqueta de HTML `img`:

```handlebars
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

#### Nombres de campo manuales

Todos los demás nombres de campo se tratan como campos rellenados manualmente.

Para crear una sección editable, agregue corchetes dobles alrededor del nombre de la sección:

```handlebars
{{customVariable}}
```

### Secciones o grupos

_Las secciones_ informan a GenStudio for Performance Marketing de que los campos de esta sección requieren un alto grado de coherencia. El establecimiento de esta relación ayuda a la IA a generar contenido que coincida con los elementos creativos de la sección.

Utilice un prefijo de su elección en el nombre del campo para indicar que un campo forma parte de una sección o grupo. Use un nombre de campo (`headline`, `body`, `image` o `cta`) después del guion bajo (`_`). Por ejemplo, el siguiente titular y cuerpo pertenecen a la sección `pod1`:

- `pod1_headline`
- `pod1_body`

Cada sección solo puede utilizar uno de cada tipo de campo. En el ejemplo anterior, la sección `pod1` solo puede usar un campo `pod1_headline`. Debido a esta regla, las secciones no se pueden anidar.

Cada tipo de plantilla, como correo electrónico o MetaAd, tiene restricciones específicas del canal en el uso de secciones. Consulte [directrices específicas del canal](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/best-practices-for-templates#follow-channel-specific-template-guidelines) en el tema _Prácticas recomendadas para usar plantillas_.

Por ejemplo, una plantilla de correo electrónico puede incluir hasta tres secciones; por lo tanto, puede tener tres secciones de titular y cuerpo:

- `pre-header`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`
- `pod3_headline`
- `pod3_body`
- `cta`

GenStudio for Performance Marketing entiende que `pod1_headline` está más relacionado con `pod1_body` que con `pod2_body`.

Consulte [Mensajes estructurados](/help/user-guide/effective-prompts.md#structured-prompts) para aprender a crear un mensaje que genere contenido variable para cada sección de un mensaje de correo electrónico.

### Llamadas a la acción

Una llamada a la acción (CTA) incluye una frase y un vínculo. Para que las capacidades de CTA _[!UICONTROL Rephrase]_ y _[!UICONTROL Add link]_ funcionen correctamente durante el proceso de generación de variantes, debe incluir marcadores de posición para el vínculo y la frase en la plantilla.

Siga estas directrices para configurar los marcadores de posición de CTA:

- La frase CTA está disponible y el vínculo puede editarse

  ```html
  <a class="button" href="{{pod1_link}}" >{{cta}}</a>
  ```

- La frase CTA está disponible, pero el vínculo **no** se puede editar porque en ella se ha proporcionado un vínculo real

  ```html
  <a align="center" href="https://link">{{cta}}</a>
  ```

- El vínculo de CTA es editable, pero la frase de reformulación **no** está disponible porque la frase se ha proporcionado en la plantilla

  ```html
  <a class="button" href="{{pod1_link}}" >Register now</a>
  ```

GenStudio for Performance Marketing también puede proporcionar frases de llamada a la acción de variante. Ver [Revisar la llamada a la acción](/help/user-guide/create/manage-variants.md#revise-call-to-action).

## Previsualización de plantilla

Al [cargar una plantilla](use-templates.md#upload-a-template), GenStudio for Performance Marketing busca en el archivo del HTML campos reconocidos. Use la vista previa para revisar los [elementos de plantilla](use-templates.md#template-elements) y confirmar que los identificó correctamente con los [nombres de campo reconocidos](#recognized-field-names).

Ejemplo de previsualización para una plantilla de correo electrónico:

![Campos de vista previa detectados](/help/assets/template-detected-fields.png){width="650"}

### Previsualización de control

Puede controlar la visibilidad del contenido especial mediante los Ayudantes integrados (expresiones especiales en el lenguaje de plantilla [!DNL Handlebars] que realizan determinadas acciones). Por ejemplo, se puede añadir una sentencia condicional que añada parámetros de seguimiento a los vínculos en la plantilla exportada, manteniendo limpios los vínculos de vista previa.

El valor `_genStudio.browser` se establece al procesar una plantilla y el valor `genStudio.export` se establece al exportar una plantilla. Puede decidir incluir cierto contenido en la parte superior de un correo electrónico mediante un envoltorio condicional, por ejemplo, cuando la plantilla se utiliza para la exportación:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Otro ejemplo puede ser evitar el uso de códigos de seguimiento al obtener una vista previa de una plantilla en GenStudio for Performance Marketing. El siguiente ejemplo muestra cómo añadir parámetros de seguimiento a los vínculos en la plantilla exportada, manteniendo limpios los vínculos de vista previa:

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## Contenido estático

Las plantillas de correo electrónico y metadatos suelen vincularse a imágenes y archivos CSS alojados en otros dominios. Cuando GenStudio for Performance Marketing genera miniaturas para vistas previas de plantillas o las experiencias derivadas de ellas, valida el origen de contenido e incrusta una copia con fines de vista previa.

Los archivos externos se incrustan temporalmente únicamente con el fin de crear la vista previa de la plantilla, lo que garantiza que la vista previa refleje con precisión el contenido tal como aparece en el momento de la creación. Estos archivos externos **no** están almacenados de forma permanente en GenStudio for Performance Marketing. Una vez creada la vista previa de la plantilla, GenStudio for Performance Marketing sigue haciendo referencia al vínculo de origen original proporcionado en la plantilla.

### Actualizar contenido

Si el origen cambia después de crear la vista previa inicial, use la función [refresh](/help/user-guide/content/use-templates.md#refresh-template) para actualizar la vista previa de la plantilla con la versión más reciente del contenido de los orígenes externos.

## Ejemplos de plantillas

+++Ejemplo: Plantilla de correo electrónico con una sección

El siguiente es un ejemplo básico de una plantilla de HTML para un correo electrónico que contiene una sección. El encabezado contiene CSS en línea simple para el estilo. El cuerpo contiene `pre-header`, `headline` y `image` [marcador de posición](#content-placeholders) que GenStudio for Performance Marketing usará para insertar contenido durante el proceso de generación de correo electrónico.

```handlebars {line-numbers="true" highlight="13"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    </div>
</body>
</html>
```

+++

+++Ejemplo: Plantilla de correo electrónico con varias secciones

La siguiente es la misma plantilla de HTML en el ejemplo anterior, pero con dos secciones más. El encabezado contiene CSS en línea para aplicar estilo a un grupo. El cuerpo usa dos grupos con [marcadores de posición de contenido](#content-placeholders) con un prefijo.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
        .pod {
            background-color: #f8f8f8;
            margin: 10px;
            padding: 20px;
            border-radius: 5px;
        }
        .pod h2 {
            color: #333;
        }
        .pod p {
            color: #666;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    <!-- Pod1 -->
        <div class="pod">
            <h2>{{ pod1_header }}</h2>
            <p>{{ pod1_body }}</p>
        </div>
        <!-- End of Pod1 -->
    <!-- Pod2 -->
        <div class="pod">
            <h2>{{ pod2_header }}</h2>
            <p>{{ pod2_body }}</p>
        </div>
        <!-- End of Pod2 -->
    </div>
</body>
</html>
```

+++

+++Ejemplo: plantilla de meta-anuncio

El siguiente es un ejemplo básico de una plantilla de publicidad Meta. El encabezado contiene CSS en línea para el estilo. El cuerpo usa [marcadores de posición de contenido](#content-placeholders) con un prefijo.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adobe</title>
    <style>
        .ad-container {
            width: 300px;
            border: 1px solid #ddd;
            padding: 16px;
            font-family: Arial, sans-serif;
        }
        .ad-image {
            width: 100%;
            height: auto;
        }
        .ad-headline {
            font-size: 18px;
            font-weight: bold;
            margin: 12px 0;
        }
        .ad-body {
            font-size: 14px;
            margin: 12px 0;
        }
        .ad-cta {
            display: inline-block;
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            text-decoration: none;
            border-radius: 4px;
            text-align: center;
        }
    </style>
</head>
<body>
<div class="ad-container">
    <img src="{{ image }}" alt="Ad Image" class="ad-image">
    <div class="ad-headline">"{{ headline }}"</div>
    <div class="ad-body">"{{ body }}"</div>
    <a href="(https://example.com)" class="ad-cta">"{{ CTA }}"</a>
</div>
</body>
</html>
```

+++
