---
title: Validación de marca en Adobe GenStudio for Performance Marketing
description: Descubra cómo funciona el sistema de validación de marca integrado en GenStudio for Performance Marketing.
feature: Brand Personalization, Variant Generation, Compliance, Content Generation, Content Review, Generative AI
exl-id: 2e777186-3b7e-46a6-9d37-7c7b7c2aa7ae
source-git-commit: 29685c96353703705f3f742e88f3934644bc4282
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Validación de marca

En GenStudio for Performance Marketing, la validación de marca es un componente esencial que funciona en colaboración con la funcionalidad y las directrices generativas de IA: [[!DNL Brands]](/help/user-guide/guidelines/brands.md), [[!DNL Products]](/help/user-guide/guidelines/products.md) y [[!DNL Personas]](/help/user-guide/guidelines/personas.md). Garantiza que todo su contenido se ajuste a la identidad de su marca, a los estándares de ADA y a la guía de plataformas de canales individuales.

GenStudio for Performance Marketing valida la marca y comprueba otros contenidos en distintos aspectos, entre ellos:

* Directrices [!DNL Brand] definidas o predeterminadas
* Directrices de Platform
<!-- * Ethical considerations related to gender, ethnicity, race, disability status, and age in AI-generated content -->
* Estándares de la Ley de Estadounidenses con Discapacidades (ADA)

## Resumen de comprobación de contenido

Se puede acceder a un resumen de la validación de marca y a otra información de comprobación de contenido para cada variante de contenido generada a través del icono de resumen _Comprobación de contenido_ para cada variante en el lienzo.

El resumen _Comprobación de contenido_ muestra:

* Porcentaje de cumplimiento de [[!DNL Brand]](brands.md) calculado como el número de [directrices](overview.md) que superaron la validación en comparación con el número de directrices probadas
* `Pass` o `Fail` resultado de las directrices de la plataforma, como Meta o LinkedIn
* `Pass` o `Fail` resultado para los estándares de accesibilidad de ADA

![Resumen de comprobación de contenido](/help/assets/content-check-summary.png){width="400" zoomable="yes"}

Haga clic en el porcentaje para ver qué tan compatible es la variante. Las puntuaciones se actualizan automáticamente a medida que realiza ediciones en las variantes. Puede hacer clic en _Ver y corregir problemas_ para garantizar una mayor conformidad.

Ver [Mejorar la alineación de la marca](#improve-brand-alignment).

## Panel de verificación de contenido

El panel _Comprobación de contenido_ se abre en el lado derecho del lienzo cuando se hace clic desde la barra de acciones derecha _o_ desde el icono de resumen [_Comprobación de contenido_](#content-check-summary) para una variante. Este panel proporciona una validación de marca detallada. las directrices de la plataforma y la información sobre los estándares de accesibilidad iluminan las oportunidades de mejora para cada sección de variante.

![Panel de verificación de contenido](/help/assets/content-check-panel.png){width="400" zoomable="yes"}

El panel _Comprobación de contenido_ muestra validación e [información de cumplimiento](/help/user-guide/guidelines/overview.md#compliance) para cada sección de la variante:

* Representación de la información de resumen de _comprobación de contenido_ para [!DNL Brand], directrices de plataforma y estándares de accesibilidad
* _Necesita revisión_ sección que muestra el número de directrices con errores e información detallada sobre cada directriz que necesita revisión
* _Pasado_ sección que muestra la cantidad de directrices aprobadas e información detallada sobre cada directriz superada

Consulte [Mejorar la alineación de la marca](#improve-brand-alignment) para obtener información sobre cómo mejorar las puntuaciones del panel _Comprobación de contenido_.

### Tipo de contenido

En el panel _Comprobación de contenido_ puede alternar las comprobaciones de pautas y estándares de accesibilidad que se deben realizar. Haga clic en el icono _Tipo de contenido_ (icono de niveles) en la parte superior del panel para activar o desactivar:

* **[!DNL Brand]**: realiza las comprobaciones asociadas con las directrices de [!DNL Brand]
* **Directrices de plataforma**: realiza las comprobaciones asociadas con la plataforma específica del canal, como Meta
* **Accesibilidad**: realiza las comprobaciones asociadas con los estándares de accesibilidad de ADA

Para **establecer el tipo de contenido** para las comprobaciones que desea realizar, haga clic para desactivar o activar los tipos disponibles y haga clic en **Aplicar**.

## Mejorar la alineación de marca

Para maximizar la eficacia del contenido generado y mantener una identidad de marca coherente, use [_Comprobación de contenido_ resumen](#content-check-summary) y [_Comprobación de contenido_ panel](#content-check-panel). Puede modificar manualmente secciones específicas para alinearlas con sus [[!DNL Brand] directrices](brands.md), comprobaciones de directrices de plataforma y comprobaciones de estándares de accesibilidad.

**Para mejorar la alineación de marca de las variantes generadas**:

1. Haga clic en el icono del panel _Comprobación de contenido_ en la barra de acciones derecha para ver la información de validación y accesibilidad de una sola variante.

   Puede ver un resumen de las comprobaciones de _Necesidades de revisión_ y _Superado_ para ver qué secciones y directrices necesitan mejorarse.

   >[!NOTE]
   >
   > La directriz _Brand voice_ indicada en el panel _Comprobación de contenido_ se aplica a toda la variante, no a una sección individual. Se resalta toda la variante de contenido para sugerir mejoras.

1. Haga clic en para corregir las directrices que actualmente no son compatibles.
1. Haga clic para expandir e inspeccionar cada comprobación que deba revisarse en secciones disponibles como _Titular_ y _Voz de marca_.

   Utilice el razonamiento proporcionado para cada comprobación para guiarle en la revisión de las variantes.

1. Después de realizar las revisiones necesarias, haga clic en **[!UICONTROL Puntuación de comprobación]** para volver a comprobar y validar los cambios y asegurarse de que estén más en consonancia con la identidad de la marca, las directrices de la plataforma y los estándares de accesibilidad.

   El proceso de comprobación de contenido se ejecuta de nuevo. Si los elementos revisados superan la validación, aparece un aviso verde en la parte inferior del lienzo para confirmar que la puntuación se ha actualizado. Si no ha habido ningún cambio después de una nueva comprobación, el banner confirma que no se ha producido ningún cambio en la puntuación. El porcentaje del icono de resumen _Comprobación de contenido_ para la variante revisada también muestra su progreso.

1. Continúe revisando las secciones para asegurarse de que toda la variante pase las comprobaciones de validación y accesibilidad. Desplácese por cada variante con las flechas adyacentes a una variante individual en el lienzo.

