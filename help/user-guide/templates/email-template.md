---
title: Directrices de plantilla de correo electrónico
description: Siga las prácticas recomendadas al utilizar plantillas de correo electrónico con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: d9d774f727b69b18af6114965fdb8ffb450f797b
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Directrices de plantilla de correo electrónico

Una plantilla de correo electrónico de marketing sirve como base para campañas de correo electrónico visualmente atractivas y adaptables. En general, las plantillas de HTML permiten controlar el diseño, la tipografía, los colores y las imágenes para alinearlos con las directrices de marca. Cuando prepare la plantilla para usarla en GenStudio for Performance Marketing, utilice HTML semántico y CSS en línea para el estilo, y evite los scripts o las dependencias externas. Las plantillas de HTML bien estructuradas pueden mejorar la experiencia del destinatario y las tasas de envío y participación.

Siga estas prácticas recomendadas de diseño al personalizar las plantillas de correo electrónico para que funcionen con GenStudio for Performance Marketing:

- Usar fuentes Adobe o Google
- Utilizar HTML y CSS en línea limpios y adaptables
- **no** usa JavaScript
- **no** usa ancho fijo en el cuerpo o contenedor
- **no** usa la codificación base64 para las imágenes porque puede aumentar significativamente el tamaño de la plantilla
- El tamaño máximo de archivo de HTML es 102 KB

## Nombres de campo reconocidos

GenStudio for Performance Marketing genera automáticamente el campo `subject` para los correos electrónicos. Al personalizar la plantilla, utilice marcadores de posición de contenido para los siguientes campos obligatorios:

- `pre_header` (texto enriquecido no habilitado)
- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (seleccionado de JPEG de contenido, PNG o GIF)

El máximo de campos permitidos en una plantilla es 20. Consulte [Marcadores de posición de contenido](/help/user-guide/content/customize-template.md#content-placeholders) para obtener más información sobre el uso de nombres de campo en las plantillas.

## Correo electrónico de varias secciones

_Las secciones_ le permiten organizar el contenido en distintos grupos, lo que admite diseños más complejos. En Genstudio for Performance Marketing, puede definir cada sección utilizando una convención de nomenclatura de grupos. Consulte [Personalizar secciones de plantilla](/help/user-guide/content/customize-template.md#sections-or-groups).

Las plantillas de varias secciones pueden tener 0, 2 o 3 secciones:

- Una plantilla básica (cero secciones) puede generar un único conjunto de elementos de plantilla, lo que no requiere la convención de nombres de grupos.
- Una plantilla compleja (varias secciones) puede generar hasta tres conjuntos de elementos de plantilla, lo que requiere que se adhiera a la convención de nomenclatura de grupos: (`groupname_fieldname`)

Ejemplo de nombres de campo para dos secciones:

- `pod1_headline`, `pod1_body`, `pod1_cta`
- `pod2_headline`, `pod2_body`, `pod2_cta`

## Ejemplos de plantillas

+++Ejemplo: Plantilla de correo electrónico con una sección

El siguiente es un ejemplo básico de una plantilla de HTML para un correo electrónico que contiene una sección. El encabezado contiene CSS en línea simple para el estilo. El cuerpo contiene `pre_header`, `headline` y `image` [marcador de posición](#content-placeholders) que GenStudio for Performance Marketing usará para insertar contenido durante el proceso de generación de correo electrónico.

```html {line-numbers="true" highlight="13"}
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
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p><a href="{{link}}">
            <img alt="{{headline}}"
                    src="{{image}}"
                    width="600" height="600"
                    border="0"/></a></p>
            <p>{{body}}</p>
        </div>
    </body>
</html>
```

+++

+++Ejemplo: Plantilla de correo electrónico con varias secciones

La siguiente es la misma plantilla de HTML en el ejemplo anterior, pero con dos secciones más. El encabezado contiene CSS en línea para aplicar estilo a un grupo. El cuerpo usa dos grupos con [marcadores de posición de contenido](#content-placeholders) con un prefijo.

```html
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
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p>{{body}}</p>
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="{{ headline }}" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="{{headline}}" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
        </div>
    </body>
</html>
```

+++
