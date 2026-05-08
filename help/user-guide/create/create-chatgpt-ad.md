---
title: Crear una experiencia publicitaria de ChatGPT
description: Aprenda a crear, revisar, publicar y activar experiencias de medios pagados de ChatGPT en Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
source-git-commit: 0f5bc2b5416193c01cc4b2fc96d9cb575e209aa3
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 9%

---


# Crear una experiencia de publicidad de ChatGPT

Use [[!DNL Create]](/help/user-guide/create/overview.md) en [!DNL GenStudio for Performance Marketing] para generar **anuncios ChatGPT** como experiencias de medios de pago, desde directrices y recursos hasta generación, comprobaciones de marca y canal, aprobación, publicación en [!DNL Content] y activación en el mismo flujo de [!DNL Activate] utilizado para canales como Meta y Google Campaign Manager 360.

Antes de empezar, [agregue directrices](/help/user-guide/guidelines/add-guidelines.md) donde sea necesario y revise [mensajes efectivos](/help/user-guide/effective-prompts.md) para que los mensajes de encabezado produzcan variantes sólidas.

## Requisitos previos

Se debe configurar según estos requisitos previos para crear o activar anuncios de ChatGPT en [!DNL GenStudio for Performance Marketing].

### Acceso y funciones

* Tiene un rol de **Editor** o superior en [!DNL GenStudio for Performance Marketing]. Consulte [Funciones de usuario y permisos](/help/user-guide/user-roles.md).
* Tiene una **cuenta de publicidad de OpenAI** y una **clave de API** de esa cuenta.
* Una cuenta de **ChatGPT Ads** está conectada a [!DNL GenStudio for Performance Marketing].

Para crear una clave de API en OpenAI Ads Manager:

1. En el Administrador de anuncios de OpenAI, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Claves de API]** > **[!UICONTROL Crear nueva clave]**.

Para conectar su cuenta de ChatGPT Ads en [!DNL GenStudio for Performance Marketing]:

1. En el área inferior izquierda, haga clic en **[!UICONTROL Más]** > **[!UICONTROL Configuración]** > **[!UICONTROL ChatGPT]** > **[!UICONTROL Conectar]** > **[!UICONTROL Agregar cuenta]**.
1. Escriba el nombre de su cuenta de publicidad de OpenAI, pegue su clave de API y haga clic en **[!UICONTROL Agregar cuenta]**.

Su cuenta de publicidad está conectada cuando el flujo se completa correctamente.

### Crear configuración

* **[!DNL Brands]**, **[!DNL Products]** y **[!DNL Personas]** están configurados para que la aplicación pueda generar una copia que no pertenezca a la marca. Ver [descripción general de las directrices](/help/user-guide/guidelines/overview.md).
* Las imágenes que desea utilizar están disponibles en [[!DNL Content]](/help/user-guide/content/overview.md).

## Generación de un anuncio de ChatGPT

Puede crear anuncios de ChatGPT como experiencias de medios pagados en el área de trabajo [!DNL Create].

### Iniciar una experiencia ChatGPT

Para abrir la creación de ChatGPT:

1. Vaya a **[!UICONTROL Crear]** > **[!UICONTROL ChatGPT]**. No selecciona plantillas para ChatGPT; se utiliza un solo diseño de anuncio.
   ![Mosaico ChatGPT en el flujo de trabajo Crear](./create-chatgpt-clp.png){width="60%"}
1. En el _lienzo_, realice selecciones para **[!DNL Brand]**, **[!DNL Product]**, **[!DNL Persona]** y **idioma**.
1. Seleccionar una imagen de [!DNL Content].
1. Escriba un mensaje para su copia de titular de ChatGPT.
1. Haga clic en **[!UICONTROL Generar]**.

[!DNL GenStudio for Performance Marketing] **genera cuatro** variantes creativas.

Puede:

* Use **[!UICONTROL Regenerar]** o **[!UICONTROL Refinar]** para ajustar el tono, la longitud o el énfasis.
* Editar texto directamente en _Lienzo_.
* Use **[!UICONTROL Intercambiar]** para elegir una imagen alternativa de [!DNL Content].

Consulte [Administrar variantes](/help/user-guide/create/manage-variants.md) para ver más formas de editar las experiencias generadas.

### Ejecución de comprobaciones de marca y canal

Antes de guardar o enviar la experiencia para su revisión, valide la copia y el diseño con las reglas de marca y canal.

Para ejecutar comprobaciones de contenido:

1. Haga clic en **[!UICONTROL Comprobación de contenido]** (comprobaciones de marca y canal).
1. Revisar los resultados de validación en el panel [_Comprobación de contenido_](/help/user-guide/guidelines/brand-validation.md#content-check-panel).
1. Resuelva los problemas marcados, como la longitud de la copia o el texto denso en pantalla, editando variantes o regenerando según sea necesario.

Consulte [Validación de marca](/help/user-guide/guidelines/brand-validation.md).

## Guardar un anuncio de ChatGPT en [!DNL GenStudio for Performance Marketing]

Guardar mueve su experiencia publicitaria de ChatGPT a [!DNL Content] para que se pueda revisar, reutilizar y activar.

Hay dos estados:

* **Experiencia de borrador** — Trabajo en curso y no aprobado.
* **Experiencia publicada** — Aprobada y disponible en [!DNL Content] para su activación.

### Enviar para revisión

1. En el encabezado de la experiencia, haga clic en **[!UICONTROL Solicitar revisión]**.
1. Seleccione aprobadores (por ejemplo, partes interesadas de la marca, legales o de rendimiento).
1. Opcional: agregue una nota en **[!UICONTROL Configuración]**.
1. Haga clic en **[!UICONTROL Enviar para revisión]**.

Los aprobadores pueden ver la experiencia ChatGPT, los resultados de las comprobaciones de marca y canal y **[!UICONTROL Aprobar]** o solicitar cambios.

Ver [Solicitar revisión y aprobación](/help/user-guide/approvals/request-review.md) y [Revisiones y aprobaciones](/help/user-guide/approvals/overview.md).

### Publicar en contenido

Después de todas las aprobaciones necesarias, publicar en [!DNL Content]:

1. Haga clic en **[!UICONTROL Publicar en contenido]**.
1. Confirme los metadatos, por ejemplo, el nombre de la campaña o la activación, la región, el idioma, el personaje, el escenario de funnel y **Canal: ChatGPT**.
1. Haga clic en **[!UICONTROL Publicar]**.

El anuncio de ChatGPT aparece en [!DNL Content] (detectable con filtros como canal o campaña) y está listo para su selección en [!DNL Activate].

Ver [Publicar contenido aprobado](/help/user-guide/approvals/publish-content.md) y [[!DNL Content] información general](/help/user-guide/content/overview.md).

## Activación de un anuncio de ChatGPT

La activación de ChatGPT utiliza el mismo módulo [[!DNL Activate]](/help/user-guide/activation/overview.md) que Meta y Google Campaign Manager 360. Consulte [Crear una activación](/help/user-guide/activation/create-activation.md) para el flujo de trabajo de activación compartida.

### Iniciar una activación de ChatGPT

Puede comenzar desde [!DNL Content] o desde [!DNL Activate].

**De[!DNL Content]**

* Seleccione una o más **experiencias publicadas** de ChatGPT.

**De[!DNL Activate]**

* Abra la tarjeta **ChatGPT** y haga clic en **[!UICONTROL + Nuevo]**.

Cada experiencia se asigna a **un** anuncio de ChatGPT.

### Configurar la configuración de experiencia

Para cada experiencia seleccionada, confirme lo siguiente:

* **Título**
* **Cuerpo**
* **Dirección URL de destino**: debe usar un formato de `https://` válido (por ejemplo, `https://www.example.com`).

### Configurar la configuración de plataforma

Seleccione los detalles del Administrador de anuncios de ChatGPT:

* **Cuenta de anuncios OpenAI**
* **ChatGPT Campaign**: ya debe existir en OpenAI Ads Manager.
* **Grupo de anuncios ChatGPT** — ya debe existir en OpenAI Ads Manager.
* **Nombre del anuncio de ChatGPT** — Un nombre distinto por anuncio de ChatGPT.

### Revisión y publicación

1. Revise todos los detalles creativos y de la plataforma.
1. Haga clic en **[!UICONTROL Publicar]**.

[!DNL GenStudio for Performance Marketing] inserta anuncios en el Administrador de anuncios de ChatGPT en un estado **inactivo**, de modo que el equipo multimedia controle el tiempo de lanzamiento final y el presupuesto, de manera consistente con otros canales de pago. Ver [Activar descripción general](/help/user-guide/activation/overview.md).

### Qué sucede después de la publicación

* Aparece un modal **publicación en curso** que se cierra automáticamente.
* Se le redirigirá a la tabla **ChatGPT Activation**, que enumera las activaciones más recientes. El estado muestra **[!UICONTROL Pendiente]** mientras se completa el procesamiento.
* Puede desplazarse fuera mientras termina la publicación.

Cuando finalice el procesamiento:

* Un elemento emergente de confirmación muestra **éxito** o **error**.
* Si hace clic en el elemento emergente (o abre la activación de ChatGPT en la tabla de activación), verá la página **Detalles**.
* Si la activación **[!UICONTROL ha fallado]**, la tabla muestra ese estado más un mensaje de error de ChatGPT.

En OpenAI Ads Manager, los equipos de medios pueden ejecutar comprobaciones finales y activar los anuncios o grupos de anuncios cuando estén listos.
