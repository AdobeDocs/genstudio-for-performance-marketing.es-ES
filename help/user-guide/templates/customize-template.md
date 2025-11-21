---
title: Personalizar una plantilla
description: Aprenda a personalizar la plantilla de HTML mediante marcadores de posición de contenido reconocidos por la IA generativa de Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation, Generative AI
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: 9f4cfd470590b2971c615a6437e6ae730cde5c18
workflow-type: tm+mt
source-wordcount: '1633'
ht-degree: 0%

---

# Personalizar una plantilla

Puede personalizar una plantilla para utilizarla en GenStudio for Performance Marketing insertando marcadores de posición o campos de contenido que la API generativa utiliza para insertar contenido.

En las siguientes secciones se explica cómo adaptar las plantillas de HTML para GenStudio for Performance Marketing utilizando el idioma de plantilla _[!DNL Handlebars]_. La sintaxis [!DNL Handlebars] utiliza texto normal con llaves dobles como marcadores de posición de contenido. Consulte [Qué es [!DNL Handlebars]](https://handlebarsjs.com/guide/#what-is-handlebars) en la_ Guía de idioma de Handlebars _para aprender a preparar la plantilla.

Una vez que la plantilla esté lista, puedes [cargarla en GenStudio for Performance Marketing](use-templates.md#upload-a-template) y empezar a generar correos electrónicos personalizados basados en la plantilla personalizada.

Siga las [directrices de accesibilidad](accessibility-for-templates.md) y las [prácticas recomendadas](/help/user-guide/templates/best-practices-for-templates.md) para que pueda llegar a más audiencia y proporcionar una experiencia óptima.

## Marcadores de contenido

>[!TIP]
>
>Los marcadores de posición de contenido **no son** iguales que el texto de marcador de posición en el contenido que un usuario debe rellenar posteriormente. Ver más acerca de [usar texto de marcador de posición en las plantillas](/help/user-guide/templates/best-practices-for-templates.md#using-placeholder-text-in-templates).

GenStudio for Performance Marketing reconoce ciertos tipos de contenido o [elementos](use-templates.md#template-elements) dentro de una plantilla, pero solo si los identifica con un [nombre de campo reconocido](#recognized-field-names).

Dentro del encabezado o del cuerpo de una plantilla de HTML, puede utilizar la sintaxis [!DNL Handlebars] para insertar un marcador de posición de contenido donde necesite que GenStudio for Performance Marketing rellene la plantilla con contenido real. GenStudio for Performance Marketing reconoce e interpreta estos marcadores de posición en función del [nombre de campo _reconocido_](#recognized-field-names). Cada nombre de campo está asociado con reglas y comportamientos específicos que determinan cómo se genera e inserta el contenido en la plantilla.

Por ejemplo, puede usar `{{headline}}` con la sintaxis [!DNL Handlebars] para indicar dónde se debe colocar el titular del correo electrónico. GenStudio reconoce este campo, genera un titular relevante basado en las directrices y los criterios de solicitud e inserta el titular en esta ubicación:

```handlebars
<div>{{headline}}</div>
```

### Nombres de campo reconocidos

En la tabla siguiente se enumeran los nombres de campo reconocidos por GenStudio for Performance Marketing para agregar un marcador de posición a una plantilla. Cada campo sigue directrices de canal específicas, instrucciones de LLM y reglas basadas en roles. Agregue estos nombres de campo con la sintaxis [!DNL Handlebars] a la plantilla donde necesita que GenStudio for Performance Marketing genere un determinado tipo de contenido.

| Campo | Función | Plantilla de canal |
| ----------------------- | ------------------------- | ------------------------------------------------ |
| `{{pre_header}}` | Preencabezado | email |
| `{{headline}}` | Titular | Enviar por correo electrónico <br>Anuncio de Meta <br>Anuncio para mostrar y titular <br>Anuncio de LinkedIn |
| `{{sub_headline}}` | Subtítulo | correo electrónico<br>Banner y anuncio en pantalla |
| `{{introductory_text}}` | Texto introductorio | Anuncio de LinkedIn |
| `{{body}}` | Copia de cuerpo | Enviar por correo electrónico <br>Anuncio de Meta <br>Anuncio en titular y en pantalla |
| `{{cta}}` | Call to action<br>Ver [llamadas a la acción](#calls-to-action) | Enviar por correo electrónico <br>Anuncio de Meta <br>Anuncio para mostrar y titular <br>Anuncio de LinkedIn |
| `{{image}}` | Imagen: seleccionar de [!DNL Content] | Enviar por correo electrónico <br>Anuncio de Meta <br>Anuncio para mostrar y titular <br>Anuncio de LinkedIn |
| `{{on_image_text}}` | En texto de imagen<br>Ver [En texto de imagen](#on-image-text). | Anuncio de Meta <br>LinkedIn |
| `{{link}}` | Call to action en la imagen<br>Ver [Vínculo en la imagen](#link-on-image). | email |

<!-- | `{{brand_logo}}`        | Logo of selected brand<br>See [Brand logo field name](#brand-logo-field-name). | email<br>Meta ad <br>LinkedIn ad | -->

GenStudio for Performance Marketing genera automáticamente ciertos campos en las siguientes plantillas:

- **La plantilla de correo electrónico** no requiere que identifique el campo `subject`
- **Meta y la plantilla** no requieren que identifique los campos `headline`, `body` y `CTA`
- **El titular y la plantilla de anuncio para mostrar** no requieren que identifique el campo `CTA`
- **La plantilla de anuncio de LinkedIn** no requiere que identifique los campos `headline`, `introductory_text` y `CTA`

>[!WARNING]
>
>En el caso de los anuncios de Instagram, el titular generado no aparece en la experiencia final.

Hay un límite de 20 campos al cargar una plantilla en GenStudio for Performance Marketing. Dado que el campo `subject` se genera automáticamente en un mensaje de correo electrónico, se cuenta como un campo. Esto significa que hay 19 campos permitidos en una plantilla de correo electrónico.

>[!TIP]
>
>Puede comprobar su plantilla con la [vista previa de la plantilla](#template-preview) en GenStudio for Performance Marketing.

### Llamadas a la acción

Un Call to action (CTA) incluye una frase y un vínculo. Para que las capacidades _[!UICONTROL Refrasear]_ y _[!UICONTROL Agregar vínculo]_ funcionen correctamente durante el proceso de generación de variantes, debe incluir marcadores de posición para el vínculo y la frase en la plantilla.

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

GenStudio for Performance Marketing también puede proporcionar frases de llamada a la acción de variante. Ver [Revisar Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action).

### Vínculo en la imagen

Puede personalizar la plantilla de correo electrónico para permitir que los creativos agreguen un vínculo a una imagen. De forma similar al vínculo de CTA, siga las instrucciones siguientes para aplicar un marcador de posición `link` a una etiqueta de imagen:

```html
<a href="{{link}}"><img src="image-source.jpg" alt="{{imageDescription}}"></a>
```

En este ejemplo:

- `{{link}}` es un marcador de posición para la dirección URL real.
- `src="image-source.jpg"` debe reemplazarse con la dirección URL real del origen de la imagen.
- `{{imageDescription}}` es un nombre de campo definido por el usuario que proporciona un marcador de posición para el texto alternativo de la imagen, el cual es útil para la accesibilidad y la optimización de los motores de búsqueda.

### Texto alternativo

Use un nombre de campo definido por el usuario como marcador de posición para generar una descripción de texto alternativo (atributo HTML `alt="text"`) para una imagen. El siguiente marcador de posición `{{imageDescription}}` se usa con el campo `{{image}}` dentro de la misma etiqueta `<img>`, lo que garantiza que la relación entre la imagen y su descripción persista.

```html
<img src="{{image}}" alt="{{imageDescription}}">
```

En este ejemplo:

- `{{image}}` es el marcador de posición para la dirección URL de origen de imagen.
- `{{imageDescription}}` es el marcador de posición del texto alternativo, que proporciona una descripción de la imagen para fines de accesibilidad y optimización de los motores de búsqueda.

### Etiqueta de accesibilidad

El atributo `aria-label` se usa para definir un nombre accesible para los elementos que no tienen etiquetas visibles. Este atributo es especialmente útil en plantillas en las que es importante proporcionar contexto para elementos interactivos, como un botón de CTA.

```html
<a class="button" href="{{link}}" aria-label="{{CTAAriaLabel}}">{{cta}}</a>
```

### En texto de imagen

El marcador de posición `{{on_image_text}}` se usa para especificar una superposición de texto de mensajes cortos e impactantes, colocados directamente en la imagen de una experiencia.

```html
<div class="image-text">{{on_image_text}}</div>
```

<!-- this field does not work in Create canvas 2025/03

### Brand logo field name

At this time, you cannot select the brand logo for the template upload. The following examples demonstrate two methods that conditionally render the brand logo. Each method verifies the source, provides a default or alternative image in case the brand logo is not available, and applies a style:

**Example 1**: Using [!DNL Handlebars] Built-in Helpers condition directly in the HTML `img src` attribute:

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Example 2**: Using [!DNL Handlebars] Built-in condition statement to wrap the HTML `img` tag:

```html
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

-->

### Nombres de campo manuales

Todos los demás nombres de campo están definidos por el usuario y se tratan como campos rellenados manualmente. Por ejemplo, puede reservar una sección para el contenido del pie de página.

Para crear una sección editable, agregue corchetes dobles alrededor del nombre de la sección:

```html
<tbody>
    <tr>
        <td>
            <p><span class="footer-text">{{footerLegal}}</span></p>
        </td>
    </tr>
</tbody>
```

### Edición de texto enriquecido

Mejore su contenido creativo durante el proceso de [!DNL Create] con la edición de texto enriquecido. El lienzo determina la capacidad del texto enriquecido en función de la ubicación del marcador de posición de contenido. La funcionalidad de texto enriquecido solo está disponible cuando se usan marcadores de posición de contenido como elementos independientes o en etiquetas HTML de nivel de bloque, como `<p>`, `<div>` o `<span>`.

La edición de texto enriquecido está disponible para contenido independiente en un párrafo:

```html
<p>{{body}}</p>
```

Si usa un marcador de posición de contenido dentro de un atributo HTML (como `alt`, `href` o `src`), no se admite la edición de texto enriquecido en ese campo.

La edición de texto enriquecido es **no** disponible para el contenido de `alt`:

```html
<img src="image.jpg" alt="{{image_description}}">
```

Si un campo aparece más de una vez, la capacidad de texto enriquecido se determina en función de si se utiliza como atributo HTML en cualquiera de las instancias. Por ejemplo, cuando el titular se utiliza como encabezado y como texto alternativo para una imagen, la etiqueta `alt` tiene prioridad.

La edición de texto enriquecido es **no** disponible para `headline` debido a que se usa como contenido de `alt`:

```html
<h1>{{headline}}</h1>
<img src="image.jpg" alt="{{headline}}">
```

La edición de texto enriquecido puede estar disponible para ciertos campos dentro de canales específicos, como `on_image_text` en canales sociales (Meta, LinkedIn).

## Secciones o grupos

Si la plantilla de correo electrónico requiere varias áreas de contenido, como varias ofertas o artículos, puede organizarlas mediante secciones o grupos. _Las secciones_ informan a GenStudio for Performance Marketing de que los campos de esta sección requieren un alto grado de coherencia. El establecimiento de esta relación ayuda a la IA a generar contenido que coincida con los elementos creativos de la sección.

Utilice un nombre de grupo de su elección como prefijo para indicar que un campo forma parte de una sección o grupo. Use un nombre de campo (como `headline`, `body`, `image` o `cta`) después del guion bajo (`_`).

Sintaxis: `groupname_fieldname`

- _Correcto_ (👍): `pod1_body`
- _Incorrecto_ (❌): `pod1body`

Cada sección solo puede utilizar uno de cada tipo de campo. Por ejemplo, los campos siguientes pertenecen a la sección `pod1`:

- `pod1_headline`
- `pod1_body`
- `pod1_image`
- `pod1_cta`

Debido a esta regla, las secciones no se pueden anidar.

Cada tipo de plantilla, como el correo electrónico o el anuncio de Meta, tiene restricciones específicas del canal en el uso de secciones. Consulte [directrices específicas del canal](/help/user-guide/templates/best-practices-for-templates.md) en el tema _Prácticas recomendadas para usar plantillas_.

Por ejemplo, una plantilla de correo electrónico puede incluir hasta tres secciones; por lo tanto, puede tener tres secciones de titular y cuerpo:

- `pre_header`
- `pod1_headline`, `pod1_body`
- `pod2_headline`, `pod2_body`
- `pod3_headline`, `pod3_body`
- `cta`

GenStudio for Performance Marketing entiende que `pod1_headline` está más relacionado con `pod1_body` que con `pod2_body`.

>[!TIP]
>
>Consulte [Mensajes estructurados](/help/user-guide/effective-prompts.md#structured-prompts) para obtener información sobre cómo crear un mensaje que genere contenido variable para cada sección en un mensaje de correo electrónico de varias secciones.

## Previsualización de plantilla

Al [cargar una plantilla](use-templates.md#upload-a-template), GenStudio for Performance Marketing busca en el archivo HTML campos reconocidos. Use la vista previa para revisar los [elementos de plantilla](use-templates.md#template-elements) y confirmar que los identificó correctamente con los [nombres de campo reconocidos](#recognized-field-names).

Ejemplo de previsualización para una plantilla de correo electrónico:

![Campos de vista previa detectados](/help/assets/template-detected-fields.png "Comprobar campos detectados"){zoomable="yes"}

Consulte [Editor de código de plantilla](/help/user-guide/templates/code-editor.md).

### Previsualización de control

Puede controlar la visibilidad del contenido especial mediante los Ayudantes integrados (expresiones especiales en el lenguaje de plantilla [!DNL Handlebars] que realizan determinadas acciones). Por ejemplo, se puede añadir una sentencia condicional que añada parámetros de seguimiento a los vínculos en la plantilla exportada, manteniendo limpios los vínculos de vista previa.

El valor `_genStudio.canvas` se establece al procesar una plantilla y el valor `genStudio.export` se establece al exportar una plantilla. Puede decidir incluir cierto contenido en la parte superior de un correo electrónico mediante un envoltorio condicional, por ejemplo, cuando la plantilla se utiliza para la exportación:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Otro ejemplo puede ser evitar el uso de códigos de seguimiento al obtener una vista previa de una plantilla en GenStudio for Performance Marketing. El siguiente ejemplo muestra cómo añadir parámetros de seguimiento a los vínculos en la plantilla exportada, manteniendo limpios los vínculos de vista previa:

```html
<a class="button" {{#if _genStudio.canvas }}
   href="{{link}}"{{/if}}{{#if _genStudio.export }}
   href="{{link}}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{cta}}</a>
```

## Contenido estático

Las plantillas de correo electrónico y Meta suelen vincularse a imágenes y archivos CSS alojados en otros dominios. Cuando GenStudio for Performance Marketing genera miniaturas para vistas previas de plantillas o las experiencias derivadas de ellas, valida el origen de contenido e incrusta una copia con fines de vista previa.

Los archivos externos se incrustan temporalmente únicamente con el fin de crear la vista previa de la plantilla, lo que garantiza que la vista previa refleje con precisión el contenido tal como aparece en el momento de la creación. Estos archivos externos **no** están almacenados de forma permanente en GenStudio for Performance Marketing. Una vez creada la vista previa de la plantilla, GenStudio for Performance Marketing sigue haciendo referencia al vínculo de origen original proporcionado en la plantilla.

### Actualizar contenido

Si el origen cambia después de crear la vista previa inicial, use la función [refresh](/help/user-guide/templates/use-templates.md#refresh-template) para actualizar la vista previa de la plantilla con la versión más reciente del contenido de los orígenes externos.
