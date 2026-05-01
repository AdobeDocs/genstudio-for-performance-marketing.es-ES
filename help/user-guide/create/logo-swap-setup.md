---
title: Configuración del intercambio de logotipos en plantillas
description: Configure los marcadores de posición del logotipo de la marca en las plantillas para habilitar el intercambio de logotipos en  [!DNL GenStudio for Performance Marketing].
feature: Create Canvas
role: User
level: Intermediate
source-git-commit: 98cb7ba338878495e6d7b68f3b8c620abae10127
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 2%

---

# Configuración del intercambio de logotipos en plantillas

Esta guía explica cómo configurar los marcadores de posición del logotipo de marca en las plantillas para habilitar la [característica de intercambio de logotipos](/help/user-guide/create/logo-swap.md) en [!DNL GenStudio for Performance Marketing]. Utilice estas directrices para asegurarse de que el marcador de posición se muestra correctamente en varios tamaños de imagen y relaciones de aspecto.

## Configuración rápida

Utilice el siguiente código de plantilla básico para la imagen de su logotipo:

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="my-logo"
>
```

Requerido:

- `src="{{brand_logo}}"`: habilita la funcionalidad de intercambio de logotipos.
- `style="{{defaultLogo}}"`: aplica el estilo de borde de marcador de posición.

Opcional:

- `class="my-logo"`: su clase CSS personalizada para cambiar el tamaño y el estilo.

## Explicación del borde del marcador de posición

Cuando no se selecciona ningún logotipo, `{{brand_logo}}` contiene una imagen transparente de 1×1 píxeles. El estilo `{{defaultLogo}}` aplica automáticamente una descripción para que el marcador de posición sea visible:

```css
outline: clamp(1px, 0.1em, 5px) dashed #FFF;
```

Comportamiento del borde:

- Aparece cuando se muestra el marcador de posición predeterminado.
- Desaparece automáticamente después de intercambiar un logotipo.
- Escala según el tamaño de fuente principal.

### Tamaño del borde

La función `clamp()` adapta el grosor del esquema al tamaño de la plantilla:

| Tamaño de fuente principal | Tamaño del esquema |
| --- | --- |
| 10px | 1 px (min) |
| 16px | 1.6px |
| 24px | 2.4px |
| 32px | 3.2px |
| 50px+ | 5 px (máx.) |

Fórmula: `0.1em` es igual al 10% del tamaño de fuente heredado, comprendido entre `1px` y `5px`.

## Personalización del borde del marcador de posición

Puede anular el esquema predeterminado mediante clases CSS. El estilo `{{defaultLogo}}` aplica el contorno base y la clase puede personalizar el color, el ancho y el estilo.

HTML de plantilla:

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-custom-border"
>
```

CSS de plantilla:

```css
.logo-custom-border {
  outline-color: #0066CC !important;
  outline-width: 2px !important;
  outline-style: dotted !important;
}
```

>[!NOTE]
>Los estilos de esquema personalizados sólo afectan al marcador de posición. Una vez que se intercambia un logotipo, todos los estilos de esquema se eliminan automáticamente.

## Definir tamaño de logotipo recomendado

Para asegurarse de que el marcador de posición esté visible y evite cambios de diseño, establezca un tamaño explícito en la clase CSS:

HTML de plantilla:

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-standard"
>
```

CSS de plantilla:

```css
.logo-standard {
  width: 120px;
  height: 60px;
}
```

## Control del posicionamiento del logotipo

Use `object-fit` y `object-position` para controlar cómo se adapta el logotipo dentro de su contenedor.

### Logotipo centrado (más común)

El logotipo se adapta a un tamaño de 150×80 píxeles, centrados horizontal y verticalmente.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-centered"
>
```

```css
.logo-centered {
  width: 150px;
  height: 80px;
  object-fit: contain;
  object-position: center center;
}
```

### Logotipo alineado a la izquierda

El logotipo se adapta, alineado con el borde izquierdo, centrado verticalmente.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-left"
>
```

```css
.logo-left {
  width: 200px;
  height: 60px;
  object-fit: contain;
  object-position: left center;
}
```

### Logo en la esquina superior derecha

El logotipo se adapta para adaptarse, colocado en la esquina superior derecha.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-top-right"
>
```

```css
.logo-top-right {
  width: 100px;
  height: 100px;
  object-fit: contain;
  object-position: right top;
}
```

## Ejemplos completos

### Configuración mínima

```html
<img src="{{brand_logo}}" style="{{defaultLogo}}">
```

>[!NOTE]
>Esta configuración funciona, pero el marcador de posición puede ser casi invisible porque la imagen transparente de 1×1 píxeles se contrae a su tamaño natural. Utilice una clase CSS con `width` y `height` para un marcador de posición visible.

### Configuración recomendada

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="brand-logo"
>
```

```css
.brand-logo {
  width: 120px;
  height: 60px;
  object-fit: contain;
  object-position: center center;
}
```

### Configuración avanzada con un borde personalizado

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="sponsor-logo"
>
```

```css
.sponsor-logo {
  width: 180px;
  height: 90px;
  object-fit: contain;
  object-position: left center;
  outline-color: #0066CC !important;
  outline-width: 2px !important;
  outline-style: solid !important;
}
```

### Configuración flexible con límites de tamaño

Utilice las propiedades `min-*` y `max-*` para plantillas adaptables o tamaños de logotipo variables.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-flexible"
>
```

```css
.logo-flexible {
  min-width: 20px;
  min-height: 20px;
  max-width: 200px;
  max-height: 100px;
  object-fit: contain;
  object-position: center center;
}
```

Cómo funciona:

- `min-width` y `min-height` mantienen visible el marcador de posición.
- `max-width` y `max-height` impiden que los logotipos de gran tamaño rompan el diseño.
- El logotipo se adapta proporcionalmente dentro de estos límites.

## Referencia de propiedades CSS

| Categoría | Propiedad | Valor | Función |
| --- | --- | --- | --- |
| Obligatorio (HTML) | `src` | `{{brand_logo}}` | Habilita la funcionalidad de intercambio de logotipos. |
| Obligatorio (HTML) | `style` | `{{defaultLogo}}` | Aplica el esquema de marcador de posición. |
| Recomendado (clase CSS) | `width` | `120px` | Establece la anchura máxima del logotipo. |
| Recomendado (clase CSS) | `height` | `60px` | Establece la altura máxima del logotipo. |
| Recomendado (clase CSS) | `object-fit` | `contain` | Ajusta el tamaño del logotipo sin recortarlo. |
| Recomendado (clase CSS) | `object-position` | `center center` | Controla la alineación del logotipo. |
| Opcional (clase CSS) | `outline-color` | `#FF0000` | Cambia el color del contorno. |
| Opcional (clase CSS) | `outline-width` | `3px` | Cambia el grosor del contorno. |
| Opcional (clase CSS) | `outline-style` | `solid` | Cambia el estilo de esquema. |
| Tamaño flexible (clase CSS) | `min-width` | `20px` | Garantiza la visibilidad del marcador. |
| Tamaño flexible (clase CSS) | `min-height` | `20px` | Garantiza la visibilidad del marcador. |
| Tamaño flexible (clase CSS) | `max-width` | `200px` | Evita el desbordamiento. |
| Tamaño flexible (clase CSS) | `max-height` | `100px` | Controla los límites del diseño. |

## Prácticas recomendadas

Haga:

- Incluya siempre `{{brand_logo}}` y `{{defaultLogo}}`.
- Defina `width` y `height` de modo que el marcador de posición sea visible.
- Utilice clases CSS para cambiar el tamaño y personalizar el esquema.
- Use `object-fit: contain` para conservar las proporciones de aspecto del logotipo.
- Prueba con logotipos de diferentes tamaños y proporciones de aspecto.

No haga lo siguiente:

- Use `border` en lugar de `outline` (el borde no se ocultará automáticamente).
- Coloque las propiedades de tamaño en los estilos en línea.
- Omitir restricciones de tamaño (el marcador de posición se procesa a 1×1 píxeles).
- Usar `object-fit: cover` (puede recortar logotipos).

## Resolución de problemas

Borde no visible:

- Asegúrese de que `style="{{defaultLogo}}"` esté incluido.
- Confirme que `width` y `height` están definidos en su clase CSS.

El marcador de posición es demasiado pequeño (1 px):

- Agregue `width` y `height` explícitos a su clase CSS.

El borde no desaparece después del intercambio:

- Utilice las propiedades de esquema en la clase CSS, no `border`.

El logotipo se recorta:

- Use `object-fit: contain` en lugar de `cover`.

Logotipo demasiado pequeño o demasiado grande:

- Ajuste `width` y `height` en su clase CSS.

No se muestra el borde personalizado:

- Confirme que `{{defaultLogo}}` se encuentra en el atributo `style`.
- Coloque las propiedades personalizadas `outline-*` en la clase CSS.
