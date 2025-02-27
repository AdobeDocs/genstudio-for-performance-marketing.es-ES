---
title: Funciones de texto
description: Obtenga información acerca de la función de texto de las categorías de atributos utilizadas en GenStudio for Performance Marketing.
feature: Insights, Attributes, Generative AI
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 5cff6d1dd097b18e4fa3d286afddc1db553a415d
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 1%

---

# Funciones de texto

Las características de texto incluyen recuentos para determinados elementos de texto, como palabras, oraciones, emojis y clasificaciones de semántica, emoción y tono que se utilizan para el análisis con [!DNL Insights]. El texto también puede recibir una puntuación de legibilidad.

GenStudio for Performance Marketing usa la IA de Adobe y las capacidades de aprendizaje automático para estudiar texto y aplicar [!UICONTROL atributos de recursos] en función de los tonos de texto y la narrativa de marketing asociados. El proceso valida el texto de entrada para asegurarse de que contiene caracteres alfanuméricos, elimina los espacios en blanco adicionales y los caracteres no imprimibles, y trunca el texto al máximo permitido de 1500 palabras. Antes de aplicar las etiquetas de atributo detectadas, la IA predice el tono predominante.

## Tono de voz

El tono representa un carácter general, una actitud o una atmósfera exhibida a través del lenguaje. Una simple elección de palabras y signos de puntuación, la estructura de la oración y el estilo pueden alterar el tono del mensaje. Por ejemplo, considere los siguientes mensajes urgentes utilizando los tres niveles básicos de tono:

- `Formal`

  ```
  Take advantage of this distinctive and exceptional opportunity!
  ```

- `Conversational`

  ```
  Don't miss out on this great opportunity!
  ```

- `Direct`

  ```
  Don't miss the chance!
  ```

La IA detecta aún más un tono más matizado. Utilizando la misma instrucción urgente del ejemplo anterior, la siguiente versión utiliza un tono `poetic` caprichoso:

- `Poetic`

  ```
  Embrace the moment, without delay, for this occasion won't always stay.
  ```

Otros valores secundarios para el tono incluyen: `Enthusiastic`, `Assertive`, `Humorous/Witty`, `Inspirational`, `Empathetic`, `Sensory`, `Storytelling`, `Poetic`, `Quantitative`, `Personal`

## Narrativa

Los atributos narrativos le ayudan a identificar recursos que comunican los valores, el propósito o la identidad que resuenan en la audiencia de destino.

| Narrativa | Descripción | Ejemplo |
| ----------------- | ----------- | ------- |
| `Authenticity` |             |         |
| `Celebration` |             |         |
| `Community` |             |         |
| `Convenience` |             |         |
| `Empowerment` |             |         |
| `Exploration` |             |         |
| `Futuristic` |             |         |
| `Hype` |             |         |
| `Indulgence` |             |         |
| `Peace of mind` |             |         |
| `Personalization` |             |         |
| `Prestige` |             |         |
| `Timelessness` |             |         |
| `Versatility` |             |         |
| `Well-being` |             |         |

## Puntuación de lectura

La puntuación de legibilidad evalúa lo fácil que es leer y comprender un fragmento de texto. Ayuda a garantizar que el contenido sea adecuado para la audiencia de destino. Las puntuaciones se basan en varios factores, incluida la longitud de la frase y la complejidad de la palabra.

| Puntuación | Nivel escolar | Notas |
| ----------- | ------------------ | ------------------------------------------------------------------------- |
| 100,00-90,00 | 5.º grado | Muy fácil de leer. Fácil de entender para un estudiante promedio de 11 años. |
| 90,0-80,0 | 6.º grado | Fácil de leer. Inglés conversacional para consumidores. |
| 80,0-70,0 | 7.º grado | Bastante fácil de leer. |
| 70,0-60,0 | 8º y 9º grado | Inglés sencillo. Fácil de entender para los estudiantes de 13 a 15 años. |
| 60,0-50,0 | De 10º a 12º grado | Bastante difícil de leer. |
| 50,0-30,0 | Universidad | Difícil de leer. |
| 30,0-0,0 | Graduado universitario | Muy difícil de leer. Mejor entendido por los graduados universitarios. |

## Recuentos de palabras

Por determinar

En la tabla siguiente se enumeran las categorías de funciones de imagen reconocidas por la API de GenStudio for Performance Marketing.

| Categoría | Descripción | Ejemplo |
| -------------------- | ------------- | --------------------- |
| Recuento de Emojis |             |        |
| Recuento de HashTags |             |        |
| Keywords |             |        |
| Emociones de marketing | Las emociones están dirigidas en los mensajes de marketing para evocar sentimientos específicos y respuestas de la audiencia, lo que puede mejorar la participación y la conexión con la marca. | `Aspiration`, `Challenge`, `Curiosity`, `Exclusivity`, `Fascination`, `Gratification`, `Recognition`, `Trust`, `Urgency` |
| Estrategias de persuasión | Técnicas utilizadas para influir en el comportamiento del consumidor y dirigir las acciones deseadas. Estas estrategias se dirigen a déclencheur psicológicos específicos y a segmentos de clientes para aumentar la efectividad de los mensajes de marketing. | `Social identity`, `Social proof`, `Endorsement`, `Concreteness`, `Foot in the door`, `Overcoming reactance`, `Reciprocity`, `Comparison`, `Social impact`, `Scarcity`, `Anthropomorphism` |
| Tono de voz | El carácter general, la actitud o la atmósfera que se transmite en un mensaje de marketing a través de la elección de palabras, la puntuación, la estructura de la oración y el estilo. | `Enthusiastic`, `Assertive`, `Humorous/Witty`, `Inspirational`, `Empathetic`, `Sensory`, `Storytelling`, `Poetic`, `Quantitative`, `Personal` |
