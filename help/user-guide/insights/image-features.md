---
title: Funciones de imagen
description: Obtenga información acerca de la función de imagen de las categorías de atributos utilizadas en GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Image Attributes, Generative AI
exl-id: b7e3d202-4085-48a4-a6ba-c950dfd52233
source-git-commit: e3534ace3679e512cce6a137aadd4c483b5a868a
workflow-type: tm+mt
source-wordcount: '1056'
ht-degree: 0%

---

# Funciones de imagen

Las características de imagen representan patrones o elementos distintos e informativos dentro de una imagen que se utilizan para el análisis con [!DNL Insights]. Estas funciones ayudan a categorizar y comprender el contenido visual, lo que permite obtener perspectivas más precisas y detalladas. Al identificar varios atributos, como el estilo, el color y los objetos, la IA puede proporcionar un análisis completo de la imagen, lo que ayuda a mejorar la toma de decisiones y la formulación de estrategias.

## Detección de estilo

Determinar el _estilo de imagen_ sirve como base para identificar otras características de la imagen. La IA puede aplicar las técnicas de análisis adecuadas y reconocer las características relevantes, lo que conduce a una comprensión más completa de la imagen. Cada estilo tiene características visuales distintas que influyen en cómo se percibe y analiza la imagen.

Si el estilo de imagen se identifica como `photograph`, la API analiza los rasgos adicionales de `camera settings`, `camera proximity` y `Photography genres`. Estos rasgos son específicos de las fotografías y proporcionan una perspectiva más profunda de la composición y calidad de la imagen. Consulta [28 tipos de estilos fotográficos](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html) en _Aprende fotografía_ de Adobe y aprende sobre tipos populares de fotografía y la terminología fundamental.

Si el estilo de imagen se identifica como `sketch` o `digital cartoon`, puede ser relevante un conjunto diferente de características. Este enfoque jerárquico garantiza que el análisis sea contextualmente preciso y se adapte al tipo específico de imagen que se examina.

## Buscar funciones de imagen

**Para ver imágenes en una categoría de atributo específica**:

1. En _[!DNL Insights]_, seleccione la vista **[!UICONTROL Atributos]**.

1. Cambie la vista de tabla seleccionando **[!UICONTROL Imágenes]**.

1. Seleccione una característica de imagen de la lista **[!UICONTROL Categoría de atributos]**, como `Scenes`.

1. Seleccione un atributo para obtener una vista detallada de las imágenes que comparten esa categoría.

   Por ejemplo, la categoría `Scenes` puede tener `restaurant` como atributo.

1. La página _Detalles del atributo_ enumera todas las imágenes con este atributo.

En la tabla siguiente se enumeran las categorías de funciones de imagen reconocidas por la API de GenStudio for Performance Marketing. La lista de atributos detectados para el contenido de medios no es exhaustiva. Los medios que contienen un conjunto completo de funciones pueden limitarse a las tres funciones más dominantes identificadas por la API.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Categoría | Descripción | Ejemplo |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Distribución de atención | Nivel de atención del visualizador distribuido en una imagen, que indica cuánto enfoque pueden recibir las distintas áreas de la imagen. Una distribución más alta significa que ninguna área domina el enfoque del espectador, mientras que una distribución más baja significa que uno o dos puntos focales capturan la atención del espectador. | `high`, `medium`, `low`<p>Ejemplo de la distribución `low` a la izquierda y la distribución `high` a la derecha:<p>![juego de pelota de distribución baja y alta](/help/assets/category/image-attn-lowhigh.png "Diferencia en la distribución baja y alta"){width="200" zoomable="yes"} |
| Ángulo de cámara | La perspectiva desde la que la cámara capta el sujeto, lo que afecta la percepción e interpretación de la imagen por parte del espectador. Si el estilo de la imagen es `photograph`, se identifica este rasgo. | `Low angle`, `High angle`, `Eye level`, `Neutral angle`, `Overhead view`, `Bird's eye view`<p>Ejemplo de `Overhead view`:<p>![Vista general](/help/assets/category/image-camera-angle.png "Par de pantalones cortos desde arriba"){width="200" zoomable="yes"} |
| Ajuste de cámara | Los ajustes y configuraciones específicos de los controles de la cámara que influyen en el aspecto final y la calidad de la imagen. Si el estilo de la imagen es `photograph`, se identifica este rasgo. | `Fast shutter speed`, `Long exposure`, `Bokeh blur`, `Motion blur`, `Tilt-shift blur`, `Flash`, `Wide-angle`, `Black and white`, `Double-exposure`, `Macro`, `Normal mode`<p>Ejemplo de configuración de `Fast shutter speed`:<p>![Velocidad de obturación rápida](/help/assets/category/image-camera-setting.png "Navegando en una ola"){width="200" zoomable="yes"} |
| Color y tono | Los colores y las cualidades tonales de una imagen. Identifica hasta tres colores de un conjunto predefinido de 40 colores en diferentes capas de imagen:<p>**[!UICONTROL Colores de primer plano]**—colores de la capa frontal de la imagen<br>**[!UICONTROL Colores de fondo &#x200B;]**—colores de la capa posterior de la imagen | Valores de color: `Red`, `Dark Red`, `Green`, `Bright Green`, `Dark Green`, `Light Green`, `Mud Green`, `Blue`, `Dark Blue`, `Light Blue`, `Royal Blue`, `Black`, `White`, `Off White`, `Gray`, `Dark Gray`, `Silver`, `Cream`, `Magenta`, `Cyan`, `Yellow`, `Mustard`, `Khaki`, `Brown`, `Dark Brown`, `Violet`, `Pink`, `Dark Pink`, `Maroon`, `Tan`, `Purple`, `Lavender`, `Turquoise`, `Plum`, `Gold`, `Emerald`, `Orange`, `Beige`, `Lilac`, `Olive` |
| Temperatura de color | Describe la calidez o la frialdad general de los colores de la imagen. | Valores de tono o temperatura: `warm`, `cool`, `neutral`<br>![colores y tonos fríos](/help/assets/category/image-color-temp.png "Temperatura de color con fondo frío y varios objetos de color"){width="200" zoomable="yes"} |
| Densidad del contenido | La concentración de elementos visuales y detalles dentro de una imagen, lo que indica cuánta información se empaqueta en el espacio visual.<p>A diferencia de la distribución de la atención, que mide cómo se propaga el enfoque del visualizador entre diferentes áreas de una imagen, la densidad del contenido se centra en la cantidad de información visual presente. Una mayor densidad de contenido significa que hay más elementos presentes. | `high`, `medium`, `low`<p>Ejemplo de `low` densidad a la izquierda y `high` densidad a la derecha:<p>![juego de pelota de baja y alta densidad](/help/assets/category/image-attn-lowhigh.png "Diferencia en la densidad de contenido baja y alta"){width="200" zoomable="yes"} |
| Estilo de imagen | El tratamiento visual de una imagen, como una fotografía o un boceto. Una vez que la IA determina el estilo de la imagen, se pueden identificar otros rasgos. Por ejemplo, si la imagen es una fotografía, pueden aplicarse los ajustes de la cámara, la proximidad de la cámara y las condiciones de iluminación. | `Photograph`, `Photograph with text overlay`, `Sketch`, `Painting`, `Digital cartoon`, `Infographics`, `Graphic design`, `Collage`, `Software screenshot`<p>Ejemplo de `digital cartoon` estilo de imagen![estilo de imagen de viñeta](/help/assets/category/image-style.png "Caricatura de estilo de imagen de un gato"){width="200" zoomable="yes"} |
| Estado de iluminación | Describe la calidad y las características de la luz de una imagen y afecta a su estado de ánimo, tono y visibilidad. | `Golden hour`, `Blue hour`, `Midday`, `Overcast`, `Night`, `Daylighting`, `Incandescent`, `Fluorescent`, `Colorful`, `Studio`<p>Ejemplo de condición `daylighting`:<p>![Persona y perro en la acera en condiciones de luz natural](/help/assets/category/image-lighting.png "Condiciones de luz natural"){width="200" zoomable="yes"} |
| Objetos | Identifica uno o más elementos, entidades y elementos que conforman la imagen. | Los valores son demasiado numerosos, pero algunos ejemplos incluyen: `backpack`, `book`, `hawk`, `glasses`, `fish`, `pencil`, `mountain bike`, `soap`<p>Ejemplo de `toucan` y `bird` objetos:<p>![pájaro, objeto de tucán](/help/assets/category/image-objects-bird.png "Diseño gráfico del objeto de ave de tucán"){width="200" zoomable="yes"} |
| Orientación | La alineación de la imagen en relación con su anchura y altura. Detecta si es más ancha que alta (horizontal), más alta que ancha (vertical) o igual en anchura y altura (cuadrada). | `landscape`, `portrait`, `square`<p>Ejemplo de orientación `square`:<p>![boceto cuadrado](/help/assets/category/image-orientation-square.png "Boceto floral de orientación cuadrada"){width="200" zoomable="yes"} |
| Personas | Cuando hay al menos una persona presente, uno o más atributos pueden describir a la persona o personas en la imagen. | `person`, `woman`, `man`, `girl`, `boy`, `social group`, `kid`, `crowd`, `people`<p>Ejemplo de personas `woman` y `person` categorías:<p>![mujer persona con cámara](/help/assets/category/image-people.png "Persona que administra una cámara"){width="200" zoomable="yes"} |
| Géneros fotográficos | Detecta el asunto y la técnica utilizados para capturar una imagen, como `Abstract` o `Landscape` (distinto de la orientación horizontal). | `Architecture`, `Astro`, `Landscape`, `Pet`, `Interior`, `Wildlife`, `Night`, `Cityscape`, `Seascape`, `Underwater`, `Storm`, `Adventure sports`, `Fashion`, `Portrait`, `Sports`, `Food`, `Street`, `Event`, `Lifestyle`, `Commercial`, `Group`, `Abstract`, `Minimalist`, `Composite`, `Surreal` <p>Ver [Tipos de fotografía](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html).<p>Ejemplo de `Adventure sports`:<p>![persona de pie con canoa](/help/assets/category/image-photography-genres.png "Persona con un remo de pie junto a una canoa"){width="200" zoomable="yes"} |
| Escenas | Identifica la configuración o el entorno de una imagen y proporciona contexto sobre dónde se capturó la imagen o el tipo de ubicación representada. | Los valores son demasiado numerosos, pero algunos ejemplos incluyen: `lake`, `underwater`, `highway`, `hill`, `log cabin`, `island`, `beach`, `lounge`<p>Ejemplo `snow`, `sky`, `winter` y `mountain` escenas reflejadas en un casco:<p>![Escena de nieve en invierno](/help/assets/category/image-scenes.png "Reflejo de invierno, nieve, cielo y montaña"){width="200" zoomable="yes"} |
| Distancia al sujeto | Distancia entre la cámara y el sujeto de una imagen. | `close up`, `mid shot`, `long shot`<p>Ejemplo de `Long shot`:<p>![Cima de montaña de tiro largo](/help/assets/category/image-subject-distance.png "Hombre en una cima de montaña distante"){width="200" zoomable="yes"} |
| Estilos | Detecta tratamientos visuales aplicados a elementos de imagen, como los utilizados en Lightroom o Photoshop. | `design`, `illustration`, `logo`, `square`, `cartoon`, `art`, `circle`, `circular`<p>Ejemplo de estilo `circular`:<p>![puerta de enlace circular en el arrecife de coral](/help/assets/category/image-styles-circular.png "Portal circular en un arrecife de coral"){width="200" zoomable="yes"} |
| Etiquetas | Detecta otras características de la imagen que no entran dentro de una clasificación específica. Las etiquetas proporcionan contexto y metadatos adicionales acerca de la imagen. Por ejemplo, la IA puede detectar `helmet` y `motorobike` objetos en una imagen e incluir `riding` como etiqueta. | Los valores son demasiado numerosos, pero algunos ejemplos incluyen: `construction`, `gothic`, `healing`, `military`, `selfie`, `football`, `typing`, `dancer`, `dancing`<p>Ejemplo de etiquetas `dancer` y `dancing`:<p>![Etiquetas para bailarín y baile](/help/assets/category/image-tags.png "Persona bailarina"){width="200" zoomable="yes"} |
