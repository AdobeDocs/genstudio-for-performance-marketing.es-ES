---
title: Directrices de plantilla de publicidad de Meta
description: Siga las prácticas recomendadas al utilizar plantillas de anuncios de Meta con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
source-git-commit: 3251d81a6bfb0c1f7d2bf3c5bd319ad4e2237699
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 1%

---

# Directrices de plantillas de anuncios Meta

Las plantillas de anuncios de Meta le ayudan a crear anuncios visualmente coherentes y eficaces en todas las plataformas de Meta. Si sigue las prácticas de diseño recomendadas y utiliza los campos compatibles, podrá asegurarse de que las plantillas estén optimizadas para GenStudio for Performance Marketing. En esta guía se explica cómo estructurar, personalizar y preparar las plantillas de publicidad de Meta para lograr una integración perfecta y resultados de alto impacto.

Siga estas prácticas recomendadas de diseño al personalizar las plantillas de anuncios de Meta para que funcionen con GenStudio for Performance Marketing:

- Utilizar una anchura de 360 píxeles para los diseños de columna
- Utilice una resolución mínima de 1080 x 1080 píxeles para las imágenes
- Se requiere exactamente un campo de imagen
- **no** usa un tamaño de fuente relativo
- **no** define la ventanilla
- **no** usa JavaScript
- **no** anula un elemento HTML en CSS
- Usar la etiqueta `<img>` en lugar de `background-image`
- Utilice el enmascaramiento para mejorar la legibilidad del texto sobre las imágenes de fondo
- Solo se puede utilizar una sección, lo que genera un único conjunto de elementos de plantilla

## Nombres de campo reconocidos

Al personalizar la plantilla de Meta ads, aplique marcadores de posición de contenido en estos campos obligatorios:

- `image` (obligatorio, seleccionado entre JPEG de contenido, PNG o GIF)
- `on_image_text` (texto que aparece sobre la imagen)

GenStudio for Performance Marketing genera automáticamente los campos siguientes. No es necesario aplicar marcadores de posición de contenido para:

- `headline`
- `body`
- `cta`

Consulte [Marcadores de posición de contenido](/help/user-guide/templates/customize-template.md#content-placeholders) para obtener más información sobre el uso de nombres de campo en las plantillas.

## Proporciones de aspecto admitidas

| Proporción de aspecto | Dimensiones (píxeles) | Notas |
|------------------|----------------------------|-----------------------------------------------------------------------|
| Cuadrado 1:1 | 1080 x 1080 | Estándar para la mayoría de las ubicaciones de Meta; recomendado para una compatibilidad amplia. |
| Vertical 4:5 | 1080 x 1350 | Optimizado para fuentes móviles; proporciona más espacio vertical. |
| Historia 9:16 | 1080 x 1920 | Ideal para historias y carretes; llena toda la pantalla móvil. |
| Horizontal 1.91:1 | 1080 x 566 | Ideal para anuncios de vínculos y ubicaciones de fuentes de noticias; formato ancho. |
| Personalizado | Mínimo de 50 x 50 (anchura) | Usar solo si es necesario; puede provocar recortes o escalas. |

Si el anuncio no está diseñado en ninguna de estas relaciones de aspecto, GenStudio for Performance Marketing recorta automáticamente la imagen en el tamaño adecuado.

## Ejemplo de plantilla

+++Ejemplo: Plantilla de anuncio de Meta

<!-- Does this need to be a precise size? -->

El siguiente es un ejemplo básico de una plantilla de publicidad de Meta. El encabezado contiene CSS en línea para el estilo. El cuerpo usa [marcadores de posición de contenido](#content-placeholders), como `image` y `on_image_text`, para indicar dónde GenStudio for Performance Marketing puede generar contenido.

```html {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Adobe</title>
        <style>
            .ad-container {
            font-family: Helvetica, sans-serif;
            position: relative;
            text-align: center;
            height: 100%;
            }
            .ad-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            }
            .ad-text {
            position: absolute;
            top: 0;
            left: 0;
            margin: 1em;
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            padding: 1em;
            font-size: 75px;
            }
        </style>
    </head>
    <body>
        <div class="ad-container">
            <img src="{{image}}" alt="Ad Image" class="ad-image" />
            <div class="ad-text">{{on_image_text}}</div>
        </div>
    </body>
</html>
```

+++
