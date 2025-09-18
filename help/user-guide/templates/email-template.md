---
title: Directrices de plantilla de correo electrónico
description: Siga las prácticas recomendadas al utilizar plantillas de correo electrónico con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: 49d8d5daa2f3c93c18cd9132dab5207871b51237
workflow-type: tm+mt
source-wordcount: '441'
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

Al personalizar la plantilla de correo electrónico, utilice marcadores de posición de contenido para los siguientes campos obligatorios:

- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (seleccionado de JPEG de contenido, PNG o GIF)

GenStudio for Performance Marketing genera automáticamente los campos siguientes. El texto enriquecido no está habilitado. No es necesario aplicar marcadores de posición de contenido para:

- `pre_header`
- `subject`

El máximo de campos permitidos en una plantilla es 20. Consulte [Marcadores de posición de contenido](/help/user-guide/content/customize-template.md#content-placeholders) para obtener más información sobre el uso de nombres de campo en las plantillas.

## Correo electrónico de varias secciones

_Las secciones_ le permiten organizar el contenido en distintos grupos, lo que admite diseños más complejos. En GenStudio for Performance Marketing, puede definir cada sección utilizando una convención de nombres de grupo. Consulte [Personalizar secciones de plantilla](/help/user-guide/content/customize-template.md#sections-or-groups).

Las plantillas de varias secciones pueden tener 0, 2 o 3 secciones:

- Una plantilla básica (cero secciones) puede generar un único conjunto de elementos de plantilla, lo que no requiere la convención de nombres de grupos.
- Una plantilla compleja (varias secciones) puede generar hasta tres conjuntos de elementos de plantilla, lo que requiere que se adhiera a la convención de nomenclatura de grupos: `<groupname_fieldname>`.
- Cuando se utilizan varias secciones, los elementos que queden independientes fuera de una sección no se rellenan.

Estos son ejemplos de nombres de campo, utilizando la convención de nomenclatura de grupos, para dos secciones:

- En la sección 1:`pod1_headline`, `pod1_body`, `pod1_cta`
- En la sección 2:`pod2_headline`, `pod2_body`, `pod2_cta`

## Ejemplos de plantillas

+++Ejemplo: Plantilla de correo electrónico con una sección

Este es un ejemplo básico de una plantilla de correo electrónico de HTML con una sección. `<head>` incluye CSS en línea simple para el estilo y `<body>` usa marcadores de posición de contenido como `pre_header`, `headline`, `sub_headline`, `body`, `cta` y `image` con vínculo y. Estos marcadores de posición permiten a GenStudio for Performance Marketing insertar contenido dinámico durante la generación de correo electrónico.

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Marketing Email</title>
        <style>
            .container {
                width: 100%;
                padding: 20px;
                font-family: Arial, sans-serif;
            }
            .cta-button {
                display: inline-block;
                background-color: #fff;
                color: #000;
                border: 2px solid #000;
                padding: 10px 20px;
                text-decoration: none;
                font-family: 'Source Sans Pro', Arial, sans-serif;
                font-weight: 600;
                font-size: 14px;
                margin-top: 20px;
                text-align: center;
            }
        </style>
    </head>
    <body>
        <div class="container">
            {{pre_header}}
            <h1>{{headline}}</h1>
            <p>
                <a href="{{link}}">
                    <img alt="banner headline" src="{{image}}" width="600" height="600">
                </a>
            </p>
            <h2>{{sub_headline}}</h2>
            <p>{{body}}</p>
            <a href="#" class="cta-button">{{cta}}</a>
        </div>
    </body>
</html>
```

+++

+++Ejemplo: Plantilla de correo electrónico con varias secciones

Esta es la misma plantilla de HTML en el ejemplo anterior, pero con dos secciones más. El encabezado contiene CSS en línea para aplicar estilo a un grupo. El cuerpo usa dos grupos con [marcadores de posición de contenido](#content-placeholders) con un prefijo.

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
            .cta-button {
            display: inline-block;
            background-color: #fff; /* Background color to white */
            color: #000; /* Text color to black */
            border: 2px solid #000; /* Border color to black */
            padding: 10px 20px;
            text-decoration: none;            
            font-family: 'Source Sans Pro', Arial, sans-serif;
            font-weight: 600; /* Semibold */
            font-size: 14px;
            margin-top: 20px;
            text-align: center;
            }
        </style>
    </head>
    <body>{{pre_header}}
        <div class="container">
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="pic1" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="pic2" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
            <a href="#" class="cta-button">{{cta}}</a>
        </div>
    </body>
</html>
```

+++
