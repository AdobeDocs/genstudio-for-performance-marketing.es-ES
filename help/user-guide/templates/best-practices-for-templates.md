---
title: Prácticas recomendadas para plantillas
description: Siga las prácticas recomendadas al utilizar plantillas con Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
TQID: https://experienceleague.adobe.com/fiKHSZ-YFZ2gSD5iZ-aKaZtsC49Mrj1dqHpHqtbXZVM
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: cc72dcf1-72e1-48cc-b434-e7c27d62d67cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 3322f783cd49ddcb897942e5e91590d53b554bdd
workflow-type: tm+mt
source-wordcount: 1347
ht-degree: 0%

---

# Prácticas recomendadas para usar plantillas

Las plantillas reducen significativamente el tiempo y el esfuerzo necesarios para generar contenido nuevo al proporcionar un punto de partida que incluye diseños y elementos de diseño preconfigurados.

Siga las siguientes recomendaciones al utilizar plantillas con GenStudio for Performance Marketing:

1. Obtenga información sobre [elementos de plantilla](#know-about-template-elements)
1. Configure [directrices de canal](#configure-channel-guidelines) para una personalización efectiva del contenido
1. Diseñe con [estándares de accesibilidad](accessibility-for-templates.md) para obtener una experiencia óptima
1. Seguir [directrices de plantillas específicas de canal](#follow-channel-specific-template-guidelines)
1. Cuando use [plantillas rápidas](/help/user-guide/templates/express-templates.md), tenga en cuenta las sugerencias específicas de [Prácticas recomendadas de plantillas de Express a GenStudio](#express-to-genstudio-template-best-practices).
>>
Conozca los conceptos básicos de los elementos y procedimientos de plantilla en [Trabajar con plantillas](use-templates.md). Y profundiza en [la personalización de una plantilla](customize-template.md) para obtener instrucciones específicas que puedes usar en tu próxima campaña.

## Uso de los elementos de plantilla adecuados

Cada tipo de plantilla utiliza diferentes elementos para crear una estructura para la creación de contenido específica del canal. [Familiarícese con las partes de una plantilla](use-templates.md#template-elements) e incluya los mejores elementos para su contenido y tipo de plantilla.

Al personalizar la plantilla, utilice los nombres de campo en lugar de estos elementos donde necesite que GenStudio for Performance Marketing genere contenido.

Ver [elementos de plantilla](use-templates.md#template-elements).

## Uso de texto de marcador de posición en plantillas

El texto de marcador de posición puede ayudar a definir la sintaxis o la estructura del contenido que un usuario debe rellenar posteriormente en una plantilla. Por ejemplo, {first_name}.{last_name}@email.etc. para definir una dirección de correo electrónico. Sin embargo, algunos delimitadores comunes ya están reservados para otros significados en GenStudio for Performance Marketing:

❌ `< >` - En uso para HTML tags.
❌ `{{ }}` - En uso para expresiones Handlebar.

Utilice corchetes sencillos (rectos o curvos) para indicar el texto del marcador de posición y evitar confusiones con las etiquetas existentes.

✅ `{first_name}` - Marcador de posición para el nombre.

## Configuración de directrices de canal

Definir directrices de canal claras es esencial para garantizar que el contenido generado se ajuste a los requisitos y objetivos de la marca. Las directrices de canal permiten especificar reglas para elementos como el tono, la longitud y el estilo que se utilizan en la plantilla. Por ejemplo, puede establecer un recuento máximo de caracteres para el cuerpo o requerir un estilo call-to-action específico. Al establecer estas directrices por adelantado, reduce la necesidad de escribir instrucciones detalladas en cada mensaje de IA, lo que optimiza el proceso de generación de contenido y garantiza la coherencia en los correos electrónicos.

Revise y defina las [directrices de canal](/help/user-guide/guidelines/brands.md#channel-guidelines) de su marca para todos los campos clave de su plantilla. Si no define directrices, se aplican las [directrices predeterminadas para canales](/help/user-guide/guidelines/brands.md#default-channel-guidelines), que pueden no reflejar completamente los requisitos de su marca.

![Especificaciones del cuerpo](/help/assets/channel-email-body.png)

Conozca de qué manera las [directrices de marcas, productos y personas](/help/user-guide/guidelines/overview.md) influyen en el contenido generado y cómo adaptarlo a sus objetivos de marketing.

## Carga de imágenes para plantillas

Las imágenes utilizadas en las plantillas deben proceder del repositorio de contenido y deben cargarse correctamente para garantizar que la imagen se muestre con precisión.

Cuando una plantilla incluye una imagen de extremo a extremo (sangrado completo), la imagen seleccionada cambia de tamaño automáticamente para ajustarse a las dimensiones completas de la plantilla. Sin embargo, si la imagen no coincide con la proporción de aspecto de la plantilla, la imagen se recorta para ajustarse a las dimensiones de la plantilla y es posible que no se muestre según lo esperado.

No hay funcionalidad de &quot;autoajuste&quot; para las imágenes incluidas en las plantillas.

Para resolver el recorte de imágenes, los usuarios deben definir la proporción de aspecto de la imagen que se utilizará en la plantilla cuando se cargue en el repositorio de contenido. Al cargar una plantilla aprobada:

1. [Continúe con el proceso de carga de plantillas](/help/user-guide/templates/use-templates.md#add-a-template) hasta que llegue a la página **[!UICONTROL Agregar detalles]**.

2. Defina la proporción de aspecto de la imagen que se usará en la plantilla en **[!UICONTROL Anchura del anuncio (px)]** y **[!UICONTROL Altura del anuncio (px)]**. Esto define la ventana de imagen para la sección de la plantilla que muestra la imagen.

3. En la sección **[!UICONTROL Más detalles]**, seleccione la lista desplegable **[!UICONTROL Tamaño de imagen]** y elija _Recortar a un tamaño fijo_.
   ![Recortado a un tamaño fijo](images/crop-to-fixed-size.png "Recortado a un tamaño fijo"){width="80%"}

Para determinar el tamaño y la proporción de aspecto de una imagen en el explorador:

1. Inspeccione la imagen.
   - En Windows/Linux:
      - Presione F12.
   - En macOS:
      - Pulse Comando + Opción + I.

1. Pase el ratón sobre la imagen.

1. Observe la relación de aspecto. Utilícelo para definir la proporción de aspecto de la imagen en la plantilla.

Cuando estos detalles no se aplican durante la carga, se asume que la imagen es toda la proporción de aspecto de la plantilla y las imágenes que no coinciden exactamente con esa proporción de aspecto aparecerán recortadas.

![Imagen recortada en un anuncio en pantalla](images/cropped-display.png "Recorte de imagen"){width="60%"}

**❌Se recortó la imagen en una plantilla de anuncio en pantalla**

![Imagen mostrada en un anuncio en pantalla](images/full-fit.png "Imagen mostrada en el anuncio en pantalla"){width="60%"}

**✅imagen completamente mostrada**

## Siga las directrices de plantillas específicas del canal

Al crear plantillas, asegúrese de que cumplen los requisitos específicos del canal al que va dirigido. Cree plantillas que se adapten al diseño y a los requisitos visuales de cada canal. Existen directrices generales que se aplican a cualquier plantilla, como:

- Utilizar HTML y CSS en línea limpios y adaptables
- Usar fuentes Adobe o Google
- **no** usa JavaScript

{{note-css-effects}}

Consulte más sugerencias y restricciones al trabajar con cada tipo de plantilla para garantizar un rendimiento óptimo:

- [Correos electrónicos](/help/user-guide/templates/email-template.md)
- [Publicidad en pantalla y banner](/help/user-guide/templates/display-template.md)
- [LinkedIn](/help/user-guide/templates/linkedin-template.md)
- [Anuncios de Meta](/help/user-guide/templates/meta-template.md)

## Prácticas recomendadas de plantillas de Express to GenStudio

Las siguientes sugerencias le ayudan a obtener resultados confiables al convertir diseños de [!DNL Adobe Express] en plantillas para [!DNL GenStudio for Performance Marketing].

### Uso de plantillas de varias variaciones

En [!DNL Adobe Express], las páginas pueden representar varias variaciones de tamaño o relación de aspecto en un archivo de plantilla.
Cuando selecciona la plantilla en [!DNL GenStudio for Performance Marketing], todas las variaciones aparecen en el lienzo.

Este comportamiento mejora con las plantillas de HTML, que solo admiten una variación por archivo.

### Bloqueo de campos para controlar lo que los especialistas en marketing pueden editar

Utilice el bloqueo para comunicar la intención. Por ejemplo, bloquee una exención de responsabilidad legal para que nunca se genere por IA, pero deje un titular flexible para la generación.

Haga clic con el botón secundario en cualquier elemento de [!DNL Adobe Express] para establecer el comportamiento del bloqueo:

- **[!UICONTROL Bloqueo completo]**: el elemento es estático y AI no genera contenido para él.
- **[!UICONTROL Bloquear, permitir reemplazo de imagen]** — Bloquea tamaño y posición, pero permite a los usuarios intercambiar la imagen. Esta opción funciona bien con logotipos.
- **[!UICONTROL Bloquear, permitir reemplazo de texto]**: bloquea el tamaño y la posición, pero permite a los usuarios editar el texto. AI no genera automáticamente contenido para él.
- **Totalmente flexible** (desbloqueado): los usuarios pueden mover y cambiar el tamaño del elemento, y AI lo trata como contenido para generar.

### Asigne nombres a las capas para una mejor asignación de IA

Al convertir un diseño en una plantilla, IA analiza el diseño y asigna campos como titular, CTA y texto independiente. La IA asigna las plantillas simples con mayor precisión que los diseños muy complejos.

**Práctica recomendada:** En la copia del marcador de posición, incluya el tipo de campo deseado (por ejemplo, `headline`, `sub-headline` o `CTA`) para ayudar a asignar correctamente los campos de IA. Este método puede reducir los errores de asignación.

### Convertir a plantilla

1. En [!DNL Adobe Express], haga clic en **[!UICONTROL Compartir]** > **[!UICONTROL Convertir en plantilla]**.
1. Solo la ficha **[!UICONTROL Información]** y **[!UICONTROL Bloqueos]** se transfieren a [!DNL GenStudio for Performance Marketing].
1. En el momento de la conversión, elija cómo funciona el desbloqueo:
   - **[!UICONTROL Permitir que los usuarios desbloqueen]**
   - **[!UICONTROL Impedir todo desbloqueo]**
   - **[!UICONTROL Establecer una frase de contraseña]**: un punto intermedio que desaconseja los cambios ocasionales sin bloquear el acceso de forma permanente.

### Mantener una copia del archivo de diseño original

La conversión crea un archivo de plantilla [!DNL Adobe Express] independiente, pero el archivo de diseño original permanece editable.

**Sugerencia:** Mantenga el original para que pueda revisar el diseño, crear variaciones y generar nuevas plantillas más adelante.

### Compartir para una mayor visibilidad

Después de la conversión, la plantilla solo es visible para usted de forma predeterminada. Puede compartirlo con particulares o con toda la organización.

**Requisito:** [!DNL Adobe Express] y [!DNL GenStudio for Performance Marketing] deben usar la misma organización de IMS para sincronizar las plantillas. Normalmente, las plantillas aparecen en [!DNL GenStudio for Performance Marketing] casi inmediatamente después de la conversión.

### Control de asignación de campos de IA

Después de seleccionar una plantilla, AI asigna campos una vez por plantilla y asigna etiquetas como **[!UICONTROL medios principales]**, **[!UICONTROL generados]** o **[!UICONTROL bloqueados]**. Puede ajustar las asignaciones manualmente cuando AI asigne los campos incorrectamente.

Use la opción **[!UICONTROL Habilitar generación]** por campo para activar o desactivar antes de generar. Puede ajustar las asignaciones manualmente cuando AI asigne los campos incorrectamente. Se han planificado correcciones permanentes en las asignaciones de plantillas para una versión futura.

### Diseño en [!DNL Adobe Express], ensamblar en [!DNL GenStudio for Performance Marketing]

Considere estos flujos de trabajo de diseño para utilizar cada servicio de la mejor manera posible:

- Trabajo de diseño completo, como colores, diseños y gráficos en [!DNL Adobe Express].
- Use [!DNL GenStudio for Performance Marketing] para ensamblar y generar contenido a partir de esas plantillas.
- Use [!DNL Adobe Express] marcas (colores, logotipos, fuentes y gráficos) para el control de diseño.
- Usar [!DNL GenStudio for Performance Marketing] marcas para los cambios de color de fuente después de la generación.

### Limitaciones de correo electrónico

El correo electrónico es **no** compatible con el lienzo Horizon para el flujo de trabajo de la plantilla [!DNL Adobe Express]. El correo electrónico sigue utilizando el proceso tradicional de plantillas de HTML.

### Aproveche las fuentes personalizadas

Los equipos suelen preguntar cómo funcionan las fuentes personalizadas con las plantillas [!DNL Adobe Express]. Es posible que los administradores tengan que aceptar la oferta correspondiente a Fuentes personalizadas en Admin Console antes de que esas fuentes estén disponibles; consulte [Usar [!DNL Adobe Express] plantillas](express-templates.md).
