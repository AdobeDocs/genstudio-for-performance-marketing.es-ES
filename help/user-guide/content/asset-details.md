---
title: Detalles del recurso
description: Adobe GenStudio for Performance Marketing almacena contenido aprobado con metadatos enriquecidos para permitir búsquedas y realizar un seguimiento del rendimiento.
feature: Attributes, Assets
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: 5e1702b26d34f519c4ab321b2adc04754fa1fcb6
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Detalles del recurso

Adobe GenStudio for Performance Marketing almacena contenido aprobado con metadatos enriquecidos para facilitar la detección y el seguimiento del rendimiento.

Cada recurso (incluidas experiencias y plantillas) tiene _detalles_ asociados (metadatos) que ayudan a identificar, rastrear, utilizar y aprender del rendimiento del contenido.

**Para ver los detalles del recurso**:

1. En _[!DNL Content]_, seleccione un recurso, experiencia o plantilla. Al hacer clic en un recurso, se abre una vista enfocada del recurso.

1. En la vista de recursos, revise la sección _[!UICONTROL Detalles]_ a la derecha.

1. Si la sección _[!UICONTROL Detalles]_ no está visible, haga clic en el icono **[!UICONTROL Información]** (i).

Los detalles del recurso incluyen los metadatos aplicados durante el proceso de creación o carga. Los tipos de metadatos de recursos incluyen [metadatos del sistema](#system-metadata) y [metadatos definidos por el usuario](#user-defined-metadata).

El siguiente recurso de imagen contiene metadatos del sistema que describen el tipo de archivo, el tamaño y otras características, una palabra clave definida por el usuario y varios atributos y colores detectados por IA.

![detalles de un recurso con varias etiquetas](/help/assets/content-asset-details.png)

>[!NOTE]
>
>Assets AEM de los repositorios de la muestran metadatos diferentes. Consulte [Configurar la visibilidad de los recursos](connect-aem-repo.md#step-4-configure-asset-visibility) para obtener información sobre cómo configurar [!DNL AEM Assets Content Hub] detalles de recursos.

## Metadatos del sistema

Algunos metadatos de recursos se recopilan automáticamente cuando se carga un recurso, como el tipo de archivo, el tamaño, las dimensiones, el origen y mucho más. Excepto por el nombre de archivo, no se pueden editar los metadatos predeterminados del sistema.

### Etiquetas generadas

Cuando almacena un recurso aprobado en [!DNL Content], GenStudio for Performance Marketing utiliza la IA de Adobe y las capacidades de aprendizaje automático para estudiar el recurso y aplicar etiquetas basadas en las funciones del recurso. Por ejemplo, la imagen de un gato puede generar etiquetas de atributos como `pet photography` o `cat`, y etiquetas de color que identifican colores dominantes en la imagen. No se pueden editar las etiquetas que se detectan y aplican automáticamente.

Consulte [!DNL Insights] [Categorías de atributos](/help/user-guide/insights/attribute-category.md) para obtener listas detalladas de las características de imagen, vídeo y texto.

### Metadatos de contenido generados

La información utilizada para generar un nuevo recurso o experiencia se convierte en metadatos, como el mensaje que se utilizó. No puede editar el mensaje una vez aprobado el contenido, pero puede utilizarlo como punto de partida para generar algo nuevo.

## Metadatos definidos por el usuario

Los metadatos definidos por el usuario añaden contexto de marketing al contenido del recurso, lo que permite a los especialistas en marketing comprender cómo utilizar el recurso y interactuar con él.

Al [cargar un recurso](/help/user-guide/content/manage-assets.md#add-assets), puede definir un conjunto de detalles de recurso opcionales que existen en GenStudio for Performance Marketing como metadatos. Incluir más detalles puede mejorar la identificación de recursos en las búsquedas y el filtrado.

### Detalles de metadatos

La siguiente tabla detalla los metadatos (detalles del recurso) que puede definir al crear un recurso.

| Campo | Descripción |
| ------------- | ----------- |
| Campañas (nombre del proyecto) | Metadatos predeterminados capturados y almacenados con el recurso |
| [!DNL Brands] | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) se agregó a GenStudio for Performance Marketing y se publicó para su uso |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md) se agregó a GenStudio for Performance Marketing para su uso |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md) se agregó a GenStudio for Performance Marketing para su uso |
| Canales | Tipos de contenido en GenStudio for Performance Marketing para los que se utiliza el recurso, como correo electrónico y anuncios Meta |
| [!UICONTROL Periodo De Tiempo] | Lapso de tiempo para el que se utiliza el recurso, como trimestre, temporada, año, etc. Ejemplo: `Winter 2023` |
| Región | Regiones para las que se utiliza el recurso. Ejemplos: `North America`, `APAC`, `Italy` |
| Idioma | Idiomas para los que se utiliza el recurso. Ejemplo: `Spanish` |
| Keywords | Palabras clave definidas por el usuario que se utilizan para la identificación adicional de características y fines del recurso |

<!-- ## History

Expand the _[!UICONTROL History]_ section to view a timeline of approvals and activity.

list other activity, show screenshot?
-->
