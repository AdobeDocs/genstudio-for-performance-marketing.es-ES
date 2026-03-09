---
title: Funciones de texto
description: Obtenga información acerca de la función de texto de las categorías de atributos utilizadas en GenStudio for Performance Marketing.
feature: Reporting and Insights, Text Attributes, Generative AI
exl-id: 7b81b0ae-0c62-468f-965c-fd8070644fb3
TQID: https://experienceleague.adobe.com/Oec5q249StCtuG-2-n1dYmJoEDRPaqLF2QANpwClQ3A
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eb30f47f-d87a-400f-8f78-63ce7979ff56
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
  - id: fc314d1d-7cb9-4a38-8dbd-8f9b6478f40d
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 1298
ht-degree: 1%

---

# Funciones de texto

Las características de texto incluyen recuentos para determinados elementos de texto, como palabras, oraciones, emojis y clasificaciones de semántica, emoción y tono que se utilizan para el análisis con [!DNL Insights]. El texto también puede recibir una puntuación de legibilidad.

GenStudio for Performance Marketing usa la IA de Adobe y las capacidades de aprendizaje automático para estudiar texto y aplicar [!UICONTROL atributos de medios] en función de los tonos de texto y la narrativa de marketing asociados. El proceso valida el texto de entrada para asegurarse de que contiene caracteres alfanuméricos, elimina los espacios en blanco adicionales y los caracteres no imprimibles, y trunca el texto al máximo permitido de 1500 palabras. Antes de aplicar las etiquetas de atributo detectadas, la IA predice el tono predominante.

## Tono de voz

El tono representa un carácter general, una actitud o una atmósfera exhibida a través del lenguaje. Una simple elección de palabras y signos de puntuación, la estructura de la oración y el estilo pueden alterar el tono del mensaje. Por ejemplo, considere los siguientes mensajes urgentes utilizando los tres niveles básicos de tono:

| Tono | Descripción | Ejemplos |
| -------------- | ----------------------------------- | --------------------------------------------------------- |
| Formal | Lenguaje pulido y profesional. | `Take advantage of this distinctive and exceptional opportunity!` |
| Conversatorio | Lenguaje amable e informal. | `Don't miss out on this great opportunity!` |
| Directo | Directo y al grano. | `Don't miss the chance!` |

Otros valores secundarios de tono proporcionan una distinción más precisa del carácter y la actitud del mensaje. De acuerdo con el ejemplo anterior de un mensaje urgente, GenAI puede detectar un tono _poético_ en este ejemplo caprichoso: `Embrace the moment, without delay, for this occasion won't always stay.`

En la tabla siguiente se enumeran los valores tonales reconocidos por la API de GenStudio for Performance Marketing.

| Tono | Descripción | Ejemplos |
| -------------- | ------------------------------------------------ | --------------------------------------------------------- |
| Asertivo | Confiado y contundente en su expresión. | `You need to act now to secure this deal!` |
| Directo | Directo y al grano. | `Don't miss the chance!` |
| Empático | Mostrar comprensión y sensibilidad. | `We understand your needs, and this is perfect for you.` |
| Entusiasta | Mostrando intenso y ansioso placer, interés o aprobación. | `This is an amazing opportunity you can't miss!` |
| Humorístico/Ingenioso | Ligero e inteligente. | `Why wait? Grab this deal before it's gone!` |
| Inspirador | Alentador y edificante. | `Believe in yourself and seize this opportunity!` |
| Poético | Artístico y expresivo. | `Embrace the dawn of a new opportunity.` |
| Cuantitativo | Según datos numéricos. | `99% of users loved this offer, and you will too.` |
| Sensorial | Engaging los sentidos. | `Feel the excitement with this incredible offer!` |
| Narración | Narrando una historia para transmitir un mensaje. | `Once upon a time, there was an offer you couldn't refuse.` |

## Atractivo emocional

Los especialistas en marketing aprovechan el poder de las emociones humanas para crear una conexión sólida entre la audiencia y la marca. Al aprovechar los sentidos como la felicidad, el miedo, la emoción o la nostalgia, los especialistas en marketing pueden crear mensajes que resuenen en un nivel más profundo, lo que impulsa la participación e influye en el comportamiento de los consumidores. El atractivo emocional ayuda a ofrecer contenido más relacionado y memorable, fomentando finalmente la lealtad a la marca y fomentando las acciones deseadas.

Las tácticas de persuasión, las emociones de marketing y los estilos narrativos trabajan juntos para dirigirse a segmentos de clientes.

- **Los estilos narrativos**, como la autenticidad, la celebración y la comunidad, ayudan a transmitir los valores y la identidad que resuenan en la audiencia de destino, lo que crea un mensaje más convincente y relacionado.
- **Las tácticas de persuasión**, como la escasez, la prueba social y la reciprocidad, están diseñadas para influir en el comportamiento del consumidor apelando a sus emociones y preferencias.
- **Las emociones de marketing** tienen como objetivo estimular sentimientos que mejoren la participación y la conexión con la marca.

La IA de GenStudio for Performance Marketing detecta y distingue estas características analizando el texto en busca de señales emocionales, tono y estilo narrativo. La IA utiliza algoritmos de procesamiento de lenguaje natural (PNL) y aprendizaje automático para identificar patrones y clasificar el texto en función de atributos emocionales y persuasivos predefinidos.

### Estilo narrativo

Los atributos de la narrativa, o factor de atractivo, ayudan a identificar medios que comunican los valores, el propósito o la identidad que resuenan con la audiencia objetivo. En la tabla siguiente se enumeran los estilos narrativos reconocidos por la API de GenStudio for Performance Marketing.

| Factor de apelación | Descripción | Ejemplos |
| ----------------- | --------------------------------------------------------------------- | ------------------------------------------ |
| Autenticidad | Genuino y real, destacando a menudo la transparencia y la honestidad. | `A behind-the-scenes look at how our products are made.` |
| Celebración | Marcando ocasiones especiales o logros con alegría y festividad. | `Join us in celebrating our 10th anniversary with special offers!` |
| Comunidad | Fomentar un sentido de pertenencia y unión entre un grupo. | `Our brand is built on the strength of our community.` |
| Comodidad | Enfatizando la facilidad de uso y las ventajas de ahorro de tiempo. | `Get what you need with just one click.` |
| Empoderamiento | Alentar y permitir a las personas tomar el control y tomar decisiones. | `Empower yourself with our latest tools and resources.` |
| Exploración | Descubrimiento y aventura atractivos, a menudo asociados con nuevas experiencias. | `Discover new horizons with our travel packages.` |
| Futurista | Resaltando la innovación y las ideas de futuro. | `Experience the future of technology today.` |
| Publicidad | Generando emoción y anticipación en torno a un producto o evento. | `Don't miss out on the most anticipated event of the year!` |
| Indulgencia | Atractivo para fantasías, deseos o placeres. | `Treat yourself to the finest gourmet chocolates.` |
| Tranquilidad mental | Proporcionar tranquilidad y una sensación de seguridad. | `Rest easy knowing your data is safe with us.` |
| Personalización | Adaptar experiencias o productos a las preferencias individuales. | `Get a custom-fit solution just for you.` |
| Prestigio | Asociarse con un alto estatus y exclusividad. | `Join the elite with our premium membership.` |
| Eternidad | Enfatizando calidad duradera y atractivo clásico. | `Our designs are timeless and never go out of style.` |
| Versatilidad | Resaltar la adaptabilidad y los usos múltiples. | `Our product fits seamlessly into any lifestyle.` |
| Bienestar | Promover la salud, la felicidad y el bienestar general. | `Enhance your well-being with our holistic approach.` |

### Tácticas de persuasión

Las técnicas de persuasión se utilizan para influir en el comportamiento del consumidor y dirigir las acciones deseadas. Estas estrategias se dirigen a déclencheur psicológicos específicos y a segmentos de clientes para aumentar la efectividad de los mensajes de marketing. En la tabla siguiente se enumeran las tácticas de persuasión reconocidas por la IA de GenStudio for Performance Marketing.

| Táctico | Descripción | Ejemplos |
| --------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| Antropomorfismo | Atribución de características humanas a productos o marcas. | `Our friendly chatbot is here to help you.` |
| Comparación | Resaltar las diferencias entre las opciones para influir en la elección. | `See how we compare to the competition.` |
| Concreción | Proporcionar detalles específicos para que el mensaje sea más tangible. | `Save 20% on your next purchase.` |
| Endoso | Con la aprobación de fuentes creíbles o influenciadores. | `Recommended by top industry experts.` |
| Pie en la puerta | Empezando por una pequeña solicitud para aumentar la probabilidad de acuerdo a una solicitud más grande. | `Try our free trial today.` |
| Superar la reactancia | Reducir la resistencia mediante el reconocimiento y el tratamiento de las objeciones. | `We understand your concerns, and here's how we address them.` |
| Reciprocidad | Ofreciendo algo de valor para alentar un favor de devolución. | `Get a free gift with your purchase.` |
| Falta | Crear una sensación de urgencia al resaltar la disponibilidad limitada. | `Only a few items left in stock!` |
| Identidad social | Aprovechamiento del sentido de pertenencia del consumidor a un grupo. | `Join our community of innovators.` |
| Impacto social | Enfatizando el impacto positivo en la sociedad o el medio ambiente. | `Your purchase helps plant a tree.` |
| Prueba social | Uso de testimonios o contenido generado por el usuario para generar confianza. | `See why thousands of users love our product.` |

### Marketing de emociones

Las emociones están dirigidas en los mensajes de marketing para evocar sentimientos específicos y respuestas de la audiencia, lo que puede mejorar la participación y la conexión con la marca. La siguiente tabla enumera las emociones reconocidas por la IA de GenStudio for Performance Marketing.

| Emoción | Descripción | Ejemplos |
| ------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| Aspiración | Inspirando un deseo de lograr o lograr algo más grande. | `Imagine the possibilities with our premium service.` |
| Desafío | Animar a la audiencia a superar un obstáculo o a aceptar una nueva tarea. | `Are you ready to take the next step in your career?` |
| Curiosidad | Despertando interés y ganas de aprender más. | `Discover the secrets behind our success.` |
| Exclusividad | Crear una sensación de ser parte de un grupo de selección. | `Join our exclusive club for members-only benefits.` |
| Fascinación | Cautivar a la audiencia con contenido intrigante o emocionante. | `Be amazed by our latest innovations.` |
| Gratificación | Proporcionar satisfacción y placer al usar el producto o servicio. | `Enjoy the ultimate comfort with our luxury bedding.` |
| Reconocimiento | Reconocer y valorar los logros o el estado de la audiencia. | `Get the recognition you deserve with our award-winning service.` |
| Confianza | Aumentar la confianza y la fiabilidad en la marca. | `Trust us to deliver quality and excellence every time.` |
| Urgencia | Impulsar la acción inmediata haciendo hincapié en las oportunidades en las que el tiempo es importante. | `Act now before this limited-time offer expires!` |

## Puntuación de lectura

La puntuación de legibilidad evalúa lo fácil que es leer y comprender un fragmento de texto. Ayuda a garantizar que el contenido sea adecuado para la audiencia de destino. Las puntuaciones se basan en varios factores, incluida la longitud de la frase y la complejidad de la palabra. En la tabla siguiente se enumeran los niveles de legibilidad reconocidos por la API de GenStudio for Performance Marketing.

| Nivel de legibilidad | Descripción | Ejemplos |
| ------------------- | ------------------------------------------------------------------ | --------------------------------------------------------- |
| 5.º grado | Lenguaje muy simple, adecuado para niños pequeños. | `The cat sat on the mat.` |
| 6.º grado | Lenguaje sencillo y claro, adecuado para una audiencia general. | `You can find great deals on our website.` |
| 7.º grado | Fácil de entender, con vocabulario y estructura directos. | `Our new product is simple to use and very effective.` |
| 8º y 9º grado | Lenguaje claro y conciso, adecuado para adolescentes. | `This guide will help you understand the basics of our service.` |
| De 10º a 12º grado | Lenguaje más complejo, adecuado para adolescentes mayores y adultos. | `The comprehensive manual provides detailed instructions for setup.` |
| Universidad | Lenguaje avanzado, adecuado para una audiencia bien educada. | `The study explores the multifaceted implications of the new policy.` |
| Graduado universitario | Lenguaje muy avanzado, adecuado para expertos y especialistas. | `The dissertation delves into the intricacies of quantum mechanics.` |

## Recuentos

Comprender y aprovechar atributos de recuento como recuentos de etiquetas, recuentos de palabras, recuentos de oraciones y proporciones de palabras de detención puede mejorar significativamente su estrategia de contenido. Estas métricas ofrecen perspectivas valiosas sobre la eficacia y el alcance de sus esfuerzos de marketing. En la tabla siguiente se enumeran las categorías de recuento reconocidas por la API de GenStudio for Performance Marketing.

| Categoría | Descripción | Ejemplos |
| --------------------- | --------------------------------------------------------------------------- | --------------------- |
| Recuento de Emojis | El número de emoji presentes en el texto. Los emojis pueden mejorar la participación y transmitir emociones rápidamente. | `😊`, `🚀`, `❤️` |
| Recuento de HashTags | El número de hashtags usados en el texto. Los hashtags ayudan a categorizar el contenido y aumentar la capacidad de detección en los medios sociales. | `#Marketing`, `#Sale` |
| Recuento de palabras por frase | El número promedio de palabras por frase en el texto. Las frases más cortas suelen ser más fáciles de leer y comprender. | `10` |
| Recuento de palabras | Número total de palabras del texto. Un mayor recuento de palabras puede proporcionar información más detallada, pero también puede requerir más esfuerzo para leer. | `1500 words` |
| Proporción de palabras de detención | Proporción entre palabras de detención y palabras significativas en el texto. Las palabras de detención (como &quot;a&quot; &quot;y&quot; &quot;the&quot;) suelen ignorarse en las consultas y resultados de búsqueda. Una alta proporción de palabras de detención puede hacer que el contenido sea menos atractivo y difícil de leer. | `0.375` |
| Recuento de frases | Número total de oraciones del texto. Las frases más largas pueden indicar un contenido más detallado, pero los textos demasiado largos pueden perder el interés del lector. | `75 sentences` |
