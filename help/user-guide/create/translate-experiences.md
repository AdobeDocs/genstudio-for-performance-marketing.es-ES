---
title: Traducción y localización de experiencias
description: Aprenda a traducir experiencias de correo electrónico y medios de pago aprobadas a varios idiomas en el lienzo de HTML en Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Content Generation
role: User
level: Beginner
source-git-commit: bc59f6f5dce0c4f22228bcd06c2f5e60a4311e04
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 2%

---

# Traducción y localización de experiencias

Adobe [!DNL GenStudio for Performance Marketing] ofrece traducción predeterminada en el lienzo de HTML para que los especialistas en marketing global y regional puedan escalar las experiencias aprobadas a varios idiomas sin herramientas de traducción externas.

La función utiliza la API abierta de Azure de forma predeterminada. Su organización también puede conectar un servicio de traducción preferido mediante [extensiones de traducción](/help/extensibility/deploy-app.md#find-translation-extensions).

La traducción comienza desde una experiencia aprobada guardada en [!DNL Content]. La experiencia de origen puede estar en cualquier idioma. Cada variante traducida se abre en el lienzo [!DNL Create] como un borrador editable que puede exportar, enviar para revisión y publicar como una experiencia independiente.

## Experiencias compatibles

La traducción predeterminada en el lienzo de HTML admite lo siguiente:

* [Experiencias de correo electrónico](/help/user-guide/create/email-experiences.md)
* Experiencias de medios de pago, incluidos anuncios de [Meta](/help/user-guide/create/meta-experiences.md), [LinkedIn](/help/user-guide/create/linkedin-experiences.md) y [Display](/help/user-guide/create/display-ad-experiences.md)

## Antes de empezar

Confirme que la experiencia que quiere traducir está **aprobada** y disponible en la galería [!DNL Content] _[!UICONTROL Experiencias]_. Las experiencias en borrador o en revisión no son fuentes de traducción aptas.

Si su organización registra una extensión de traducción personalizada, GenStudio for Performance Marketing utilizará ese servicio en lugar de la traducción predeterminada de Azure Open AI. Ver [Buscar extensiones de traducción](/help/extensibility/deploy-app.md#find-translation-extensions).

## Traducir de [!DNL Create] {#translate-from-create}

Inicie una traducción de la página de aterrizaje [!DNL Create] para localizar una experiencia aprobada.

![Traducir y localizar la copia en la página Crear página de aterrizaje](./translate-create-workflow.png){width="600" zoomable="yes"}

**Para traducir desde[!DNL Create]**:

1. En [!DNL Create], desplácese hasta la sección _Creación de contenido_.
1. Haga clic en **[!UICONTROL Traducir y localizar copia]**.
1. Seleccione la experiencia de correo electrónico o medios de pago aprobados que desee traducir. Haga clic en el botón **[!UICONTROL Usar]**.
1. Seleccione los idiomas de destino de la lista de idiomas admitidos. Haga clic en **[!UICONTROL Traducir]**.

Las variantes traducidas aparecen en el lienzo.

## Traducir de [!DNL Content] {#translate-from-content}

También puede iniciar la traducción de [!DNL Content] cuando esté explorando experiencias aprobadas.

### Desde la galería Experiencias

![Acción de traducción en una experiencia de la galería de contenido](./translate-content-gallery.png){width="500" zoomable="yes"}

**Para traducir desde la galería de experiencias**:

1. En [!DNL Content], abra la ficha **[!UICONTROL Experiencias]**.
1. Busque la experiencia aprobada que desea traducir.
1. Haga clic en el menú opciones (tres puntos) de la tarjeta de experiencia.
1. Haga clic en **[!UICONTROL Traducir]**.
1. Seleccione los idiomas de destino de la lista de idiomas admitidos. Haga clic en **[!UICONTROL Traducir]**.

## Trabajo con traducciones en el lienzo

En el lienzo de HTML, la experiencia de origen no se puede editar porque ya está aprobada. Las experiencias de origen de correo electrónico aparecen bloqueadas. Puede editar texto en variantes traducidas directamente en el lienzo. Consulte [Administrar variantes](/help/user-guide/create/manage-variants.md) para obtener instrucciones sobre cómo editar una copia de variante.

Las experiencias traducidas no ejecutan la validación de marca ni muestran una puntuación de marca. La experiencia de origen ya se ha creado con directrices de marca, revisado y aprobado.

La regeneración de fragmentos no es compatible con las experiencias traducidas.

### Eliminar un idioma traducido

**Para quitar un idioma traducido del lienzo**:

1. En el lienzo [!DNL Create], haga clic en el menú de opciones (tres puntos) en el encabezado de variante traducido.
1. Haga clic **[!UICONTROL eliminar]**.

![Eliminar un idioma traducido del lienzo](./remove-translation-variant.png){width="500" zoomable="yes"}

El idioma traducido se elimina del lienzo.

### Actualizar una traducción de medios de pago

Después de editar la copia de medios de pago traducida, puede volver a cargar la salida de traducción original.

**Para actualizar una traducción de medios pagados**:

1. En el lienzo [!DNL Create], abra el menú de opciones en la variante traducida editada.
1. Haga clic en **[!UICONTROL Actualizar traducción]**.

>[!NOTE]
>
>La traducción de actualización está disponible para experiencias de medios de pago. La traducción por correo electrónico no admite la actualización de la traducción en este momento.

## Exportar, revisar y publicar

Una vez que las traducciones se carguen en el lienzo, podrá exportarlas, enviarlas para su aprobación y publicar las variantes aprobadas en [!DNL Content].

**Para exportar experiencias traducidas**:

1. En el lienzo [!DNL Create], haga clic en **[!UICONTROL Exportar]** en la barra de herramientas.
1. Seleccione un formato de exportación.
   * Correo electrónico: **CSV e imágenes** o **solo HTML**
   * Medios de pago: **CSV + JPG**, **CSV + PNG** o **HTML + imágenes**
1. Haga clic en **[!UICONTROL Exportar]**.

También puede [exportar experiencias de [!DNL Content]](/help/user-guide/content/manage-assets.md#export-experiences).

**Para solicitar revisión y aprobación**:

1. En el lienzo [!DNL Create], haga clic en **[!UICONTROL Solicitar aprobación]**.
1. Asigne al menos un aprobador y envíe la solicitud.

Consulte [Solicitar revisión y aprobación](/help/user-guide/approvals/request-review.md) para obtener detalles sobre el flujo de trabajo de revisión.

**Para publicar traducciones aprobadas**:

1. Una vez que los aprobadores aprueben las variantes traducidas, haga clic en **[!UICONTROL Publicar]**.
1. En la ventana de publicación, confirme los metadatos, como el nombre de la campaña, los periodos de tiempo, las regiones y las palabras clave.

Ver [Publicar contenido aprobado](/help/user-guide/approvals/publish-content.md).

Cada traducción publicada se guarda en [!DNL Content] como una experiencia independiente.

## Metadatos de la experiencia traducida

Las traducciones publicadas incluyen metadatos que vinculan cada variante con su origen, lo que incluye:

* **Título** — sigue el patrón `Translation from "<source title>" <channel>`, como `Translation from "Summer campaign" Meta`
* **Creado por** — el usuario que inició la traducción
* **Fecha de creación** — la fecha de la traducción
* **Origen traducido**: un vínculo a la experiencia de origen en [!DNL Content]
* **Traducido de** — el idioma de origen

## Limitaciones

Tenga en cuenta las siguientes restricciones al traducir experiencias en el lienzo de HTML:

* La experiencia de origen ya debe estar aprobada y guardada en [!DNL Content].
* La validación de marca no se ejecuta en variantes traducidas.
* La regeneración de fragmentos no es compatible con las experiencias traducidas.
* La traducción de actualización solo está disponible para medios de pago.

## Información relacionada

* [Experiencias de correo electrónico](/help/user-guide/create/email-experiences.md)
* [experiencias de Meta](/help/user-guide/create/meta-experiences.md)
* [Mostrar experiencias de anuncios](/help/user-guide/create/display-ad-experiences.md)
* [Administrar recursos y experiencias](/help/user-guide/content/manage-assets.md)
* [Buscar extensiones de traducción](/help/extensibility/deploy-app.md#find-translation-extensions)
