---
title: Funciones de vídeo
description: Obtenga información acerca de la función de vídeo de las categorías de atributos utilizadas en GenStudio for Performance Marketing.
feature: Insights, Attributes, Generative AI
source-git-commit: f8b22221f4fee0e1430740e670f580926ac33862
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 1%

---

# Funciones de vídeo

Las características de vídeo representan elementos, sonidos o patrones distintos e informativos dentro de un vídeo para su análisis con [!DNL Insights]. Estas funciones ayudan a categorizar y comprender el contenido del vídeo, lo que permite obtener perspectivas más precisas y detalladas. Al identificar varios atributos, como el estado de ánimo del audio, el género musical y los objetos, la IA puede proporcionar un análisis exhaustivo del vídeo, lo que ayuda a mejorar la toma de decisiones y la formulación de estrategias.

## Detección de audio

La detección de audio en GenStudio for Performance Marketing implica el análisis de la pista de audio de un vídeo para identificar varios atributos. Este proceso de detección determina el estado de ánimo general del audio mediante la identificación de los tipos de audio presentes, el etiquetado de géneros específicos o categorías de música, y la extracción de palabras clave del habla. Al comprender estos elementos de audio, la IA puede proporcionar una perspectiva más profunda del contenido y el contexto del vídeo, mejorando el proceso general de análisis y categorización.

## Buscar funciones de vídeo

**Para obtener una vista previa de un vídeo y escuchar una muestra del audio**:

1. En _[!DNL Insights]_, seleccione la vista **[!UICONTROL Atributos]**.

1. Cambie la vista de tabla seleccionando **[!UICONTROL Vídeo]**.

1. Seleccione una característica de la lista **[!UICONTROL Categoría de atributos]**. Para ver un ejemplo de audio, selecciona **Género musical**.

1. Seleccione un atributo para obtener una vista detallada de los vídeos que comparten esa categoría.

   Por ejemplo, la categoría `Music genre` puede tener `electronic` como atributo.

1. La página _Detalles del atributo_ enumera todos los vídeos con este atributo. Mantenga el puntero del ratón sobre cualquier vídeo de la lista para iniciar una previsualización de vídeo.

1. Cambie el botón **reactivar el silencio** (ubicado en la esquina inferior izquierda de una vista previa de vídeo) y escuche el audio de la vista previa del vídeo.

En la tabla siguiente se enumeran las categorías de funciones de vídeo reconocidas por la API de GenStudio for Performance Marketing. La lista de atributos detectados para un recurso no es exhaustiva. Las Assets que contienen un conjunto completo de funciones pueden limitarse a las tres funciones más dominantes identificadas por la API.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Categoría | Descripción | Ejemplo |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| Modo de audio | Determina el tono emocional general o la atmósfera de la pista de audio, como `calm`, `upbeat` o `tense`. | `Energetic`, `Happy`, `Emotional Ambient/atmospheric`, `Relaxing`, `Dramatic`, `Expressive/characterful`, `Intense`, `Slow`, `Neutral` |
| Tipos de audio | Etiqueta el vídeo con uno o más tipos de audio presentes, como `music` o `speech`. | `Music`, `Speech`, `Silence`, `Special effects`, `Ambience` |
| Categorías | Clasifica el vídeo en una o más categorías de contenido amplias. | `Entertainment`, `Sports`, `Music`, `Gaming`, `Howto tutorials`, `Fashion and style`, `Film and animation`, `Science and technology`, `Autos and vehicles`, `Pets and animals`, `People and blogs`, `News and politics`, `Social causes and activism`, `Travel and events`, `Education`, `Sales and offers` |
| Categoría de música | Amplia clasificación del género musical cuando la música está presente en el vídeo. Esto ayuda a identificar el tipo general de música, como los estilos `contemporary` o `traditional`. | `Contemporary/pop music`, `Traditional/folk-based music`, `Instrumental/orchestral music`, `Rock music`, `Acoustic/unplugged music`, `Specialised/occasional music`, `Experimental/unique music` |
| Género musical | Clasificación específica del estilo de música cuando hay música en el vídeo, que proporciona una identificación más detallada de la música, como `electronic` o `jazz`. | `electronic`, `hip-hop`, `dance`, `novelty`, `rock`, `world`, `reggae`, `pop`, `film`, `jazz`, `background`, `latin` |
| Objetos | Identifica uno o más elementos, entidades y elementos que aparecen en el vídeo. | Los valores son demasiado numerosos, pero algunos ejemplos incluyen: `backpack`, `book`, `hawk`, `glasses`, `fish`, `pencil`, `mountain bike`, `soap` |
| Orientación | La alineación del vídeo en relación con su anchura y altura. Detecta si es más ancha que alta (horizontal), más alta que ancha (vertical) o igual en anchura y altura (cuadrada). | `landscape`, `portrait`, `square` |
| Personas | Cuando hay al menos una persona presente, uno o más atributos pueden describir a la persona o personas presentes en el vídeo. | `person`, `woman`, `man`, `girl`, `boy`, `social group`, `kid`, `crowd`, `people` |
| Escenas | Identifica la configuración o el entorno de un vídeo y proporciona contexto sobre dónde se realizó el vídeo o el tipo de ubicación representada. | Los valores son demasiado numerosos, pero algunos ejemplos incluyen: `lake`, `underwater`, `highway`, `hill`, `log cabin`, `island`, `beach`, `lounge` |
| Estilos | Detecta tratamientos visuales aplicados a elementos de vídeo, como los utilizados en After Effects o Lightroom. | `design`, `illustration`, `logo`, `square`, `cartoon`, `art`, `matte`, `neon` |
| Etiquetas | Detecta otras características de vídeo que no entran dentro de una clasificación específica. Las etiquetas proporcionan contexto y metadatos adicionales acerca del vídeo. | Los valores son demasiado numerosos, pero algunos ejemplos incluyen: `construction`, `gothic`, `healing`, `military`, `selfie`, `football`, `typing`, `dancer`, `dancing` |
