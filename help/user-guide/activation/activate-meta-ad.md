---
title: Activar un anuncio de Meta
description: Obtenga información sobre cómo activar una experiencia de anuncio de Meta.
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
source-git-commit: 0ccdeb2b3375e9ee72bfc4458eeaff11709768cb
workflow-type: tm+mt
source-wordcount: '1907'
ht-degree: 1%

---

# Activar un anuncio de Meta

Adobe GenStudio for Performance Marketing admite la activación de experiencias de anuncios de Meta en Instagram y Facebook.

Puede [crear una experiencia de Meta](/help/user-guide/create/create-meta-ad.md) en GenStudio for Performance Marketing y seleccionarla para su activación, o construir una nueva experiencia a partir de recursos aprobados en [!DNL Activate].

La activación de un anuncio de Meta sigue los [mismos pasos generales](create-activation.md) necesarios para la activación en otros canales de pago. El proceso de activación permite preparar la experiencia publicitaria para los requisitos específicos de Meta. Después de activar una experiencia de Meta en GenStudio for Performance Marketing, use [Meta Ads Manager](https://adsmanager.facebook.com/) para ajustar la experiencia en ubicaciones de anuncios de Meta específicas antes de la publicación final.

Los administradores de sistemas y editores de GenStudio pueden activar las experiencias publicitarias.

## Paso 1: Configuración de las cuentas de Meta

Antes de iniciar una activación, [inicia sesión en Meta](https://adsmanager.facebook.com/) para acceder a tu cuenta de Meta Ads Manager.

>[!BEGINSHADEBOX]

**Requisitos previos**:

Confirme que las cuentas de publicidad de Meta conectadas tienen permiso total para administrar los anuncios de estos componentes de Meta Advertising Platform:

* Página de Facebook
* campaña de Meta
* Conjunto de anuncios de Meta
* Perfil de Instagram (opcional)

>[!ENDSHADEBOX]

## Paso 2: Conéctese a sus cuentas de Meta

Para que su organización pueda activar experiencias, un administrador del sistema de GenStudio debe conectar sus cuentas de Meta a GenStudio for Performance Marketing. Esta conexión permite que los datos fluyan entre GenStudio y las herramientas de marketing externas como Meta, lo que permite el proceso de activación.

Ver [Conectarse a Meta Ads](/help/user-guide/connectors/meta-ads.md).

Una vez finalizada la sincronización, puede ver las cuentas añadidas. Las grandes cantidades de datos tardan más en sincronizarse.

## Paso 3: Prepare su experiencia para la activación

Puede iniciar una activación de dos formas:

* **Activar directamente desde[!DNL Content]**. La selección de una experiencia aprobada con una configuración predefinida es la forma más sencilla de iniciar una activación en un solo canal.

* **Organice su experiencia publicitaria desde [!DNL Activate] > _Configuración de experiencias_**. Puede crear una experiencia seleccionando recursos visuales de [!DNL Content], agregando elementos de texto y relaciones de aspecto. Este enfoque tiene más pasos, pero proporciona una mayor flexibilidad al crear su experiencia creativa.

### Activar una experiencia aprobada desde el contenido

Puede seleccionar más de una experiencia para activarla en un solo canal de pago. Se le puede pedir que seleccione una plataforma antes de continuar con la activación.

Si ha seleccionado más de una experiencia para activarla como grupo, utilice la barra lateral izquierda para enfocar la vista de _Configuración de experiencias_ en los detalles de la experiencia seleccionada.

1. Use las herramientas de búsqueda y filtrado de la galería [!DNL Content] para identificar la experiencia que desea activar y luego haga clic en **[!UICONTROL Activar]**.

   Se abre la página de Meta ads _Experience setup_ para esta experiencia. Ya contiene los detalles de la experiencia seleccionada. Puede editar los campos **[!UICONTROL Call-to-action]**, **[!UICONTROL URL del sitio web]** y **[!UICONTROL Vínculo de visualización]**. Si selecciona más de una experiencia para activar, la vista _Configuración de experiencias_ incluye una barra lateral izquierda que muestra miniaturas de todas las experiencias seleccionadas. Utilice esta barra lateral izquierda para enfocar la vista de _Configuración de experiencias_ en los detalles de la experiencia seleccionada.

1. Seleccione una campaña en el menú desplegable **[!UICONTROL Campañas]**.

   Si está trabajando con varias experiencias, alterne entre experiencias en la barra lateral izquierda hasta que haya completado la preparación de cada experiencia.

1. Haga clic en **[!UICONTROL Siguiente]** para confirmar la configuración de los anuncios de Meta.

1. Asigne un nombre a cada experiencia. Después de la activación, puede usar este nombre para buscar esta experiencia en la tabla de _experiencias activadas_.

### Montar componentes de experiencia

Si decide no activar directamente una experiencia aprobada de [!DNL Content], puede seleccionar recursos, asignar proporciones de aspecto y elementos de texto de borrador.

**Para preparar tu experiencia para la activación**:

1. Desde [!DNL Activate], haz clic en **[!UICONTROL Nuevo]** en el icono que representa el canal de pago que hayas elegido. Se abre la vista _Configuración de experiencias_.

   La página _Configuración de experiencias_ proporciona una ubicación central para preparar la activación de anuncios. La preparación del anuncio incluye estas tres tareas:

1. Asigne un nombre a su experiencia. Después de la activación, puede usar este nombre para buscar esta experiencia en la tabla de _experiencias activadas_.
1. Seleccione recursos de medios. Puede usar recursos de [!DNL Content] o cargar recursos externos (por ejemplo, de OneDrive o Dropbox).
1. [Agregar texto](#add-ad-text).
1. [Agregar metadatos](#assign-metadata).

   El _panel de vista previa_ admite una vista interactiva del texto y los recursos en el contexto de una ubicación de anuncio específica. Utilice el menú desplegable _Seleccionar ubicación_ para cambiar entre las ubicaciones de anuncios compatibles. Las vistas previas proporcionan la oportunidad de finalizar decisiones sobre elementos de publicidad para ubicaciones específicas. Al seleccionar una ubicación en el panel _Vista previa_, solo se ve afectada la vista del anuncio. No se ha guardado su selección de ubicación en el panel _Vista previa_.

### Selección de los recursos multimedia

Utilice la sección _Medios_ para seleccionar al menos un recurso de imagen para incluirlo en su experiencia. Las ubicaciones de anuncios están asociadas con proporciones de aspecto de imagen admitidas, que se enumeran como opciones en el menú desplegable _Ubicaciones_. Este menú muestra las ubicaciones de anuncios compatibles para publicaciones de Facebook o historias de Instagram, organizadas por proporción de aspecto.

Después de la carga, los recursos se guardan en [!DNL Content]. El área _Media_ muestra la imagen de forma predeterminada con una proporción de aspecto de 1:1. Las relaciones de aspecto alternativas incluyen solo los valores admitidos por el canal de publicidad de pago. Se agrupan por orientación vertical y horizontal. GenStudio for Performance Marketing admite la inclusión de hasta seis relaciones de aspecto por experiencia activada.

**Para cargar un recurso desde el contenido**:

[!DNL Content] proporciona una vista central para los recursos y las experiencias aprobados de su organización. Puede enfocar el inventario mostrado de recursos de [[!DNL Content] gallery](/help/user-guide/content/manage-assets.md) mediante las opciones de menú **[!UICONTROL Buscar]** (lupa) y _Filtrar_.

1. Desde [!DNL Activate], haga clic en **[!UICONTROL Nuevo]** en la tarjeta del canal. Se abre la vista _Configuración de experiencias_.

1. Haga clic en **[!UICONTROL Seleccionar]** y, a continuación, seleccione **[!UICONTROL Seleccionar del contenido]**. Se abre la vista _Seleccionar contenido_, que muestra una galería de recursos de imagen que puede filtrar o buscar.

1. Utilice las herramientas de búsqueda y filtrado de la galería [!DNL Content] para seleccionar al menos un recurso para cargar.

1. Haz clic en **[!UICONTROL Usar]** para incluir el recurso seleccionado en tu experiencia publicitaria. La ventana _Configuración de experiencias_ incluye el recurso en su proporción de aspecto predeterminada en el área _Medios_. El panel _Vista previa_ obtiene una vista previa del recurso en la ubicación del anuncio que admite esta relación de aspecto.

Si la carga no se ha realizado correctamente, se abrirá un mensaje de error informativo que incluye un vínculo al recurso en _[!DNL Content]_.

**Para cargar un recurso externo**:

Puede cargar hasta seis imágenes estáticas externas a la galería [!DNL Content] desde Microsoft OneDrive o Dropbox.

1. En [!DNL Activate], haga clic en **[!UICONTROL Nuevo]** en el mosaico de Meta. Se abre la ventana _Configuración de experiencias_.

1. En la sección _Medios_, haga clic en **[!UICONTROL Seleccionar]**. Un menú desplegable muestra opciones para _Seleccionar entre el contenido_ o _Cargar_.

1. Haga clic en **[!UICONTROL Cargar]** Se abre la ventana _Agregar proporciones de aspecto_.

1. Para seleccionar imágenes en las relaciones de aspecto admitidas, arrastre y suelte los archivos de imagen en el área de carga de imágenes. También puede examinar el dispositivo en busca de recursos.

1. (Opcional) Para cargar recursos desde su dispositivo, haga clic en **[!UICONTROL Examinar]** y, a continuación, seleccione _Examinar archivos_ o _Examinar carpetas_ para identificar los recursos que se van a cargar.

1. En el área _Agregar detalles_, agregue detalles informativos a los recursos cargados para facilitar la búsqueda y el filtrado en _[!DNL Content]_. Estos detalles se guardan como metadatos.

1. Cuando haya cargado los recursos y asignado los detalles, haga clic en **[!UICONTROL Agregar Assets]** en la parte inferior derecha.

### Añadir texto del anuncio

Utilice la sección _Texto_ de la página _Activar anuncio de Meta_ para agregar texto atractivo y compatible con la marca a los campos de texto requeridos. Texto incluye el texto principal (cuerpo) del anuncio y el texto de call-to-action. No puede editar los campos _Texto principal_, _Titulares_ y _Descripción_. Puede editar los campos _Call-to-action_, _Vínculo de visualización_ y _Dirección URL del sitio web_.

| Campo | Requerido | Límite de caracteres (máximo) |
|-----------------|---------------------------|---------------------------------|
| Nombre del anuncio | sí | 500 |
| Texto principal | sí | 500 |
| Titular | sí | 255 |
| Descripción | no | 125 |
| Call to action | sí | solo opciones del menú desplegable |
| Mostrar URL | no | 1000 |
| URL del sitio web | sí | 1000 |
| Imagen | se requiere al menos uno |                                 |

GenStudio for Performance Marketing requiere _texto principal_ y _título_, no Meta.

### Asignar metadatos

Los detalles de la experiencia se guardan como metadatos y ayudan a los usuarios a buscar una experiencia. Estos detalles aumentan la visibilidad de la experiencia en [!DNL Content]. Utilice estos detalles opcionales definidos por el usuario para identificar el propósito de la experiencia y el contexto o las campañas en las que se implementa.

| Detalle | Descripción |
|------------|-------------|
| Campañas | Todas las campañas de GenStudio for Performance Marketing a las que pertenece la experiencia publicitaria. |
| Marca | Directrices, definidas por el usuario o predeterminadas, que permiten a los usuarios establecer directrices de marca que capturan la esencia de la identidad de una marca. |
| Productos | Productos asociados a su organización e identificados en GenStudio for Performance Marketing |
| Personas | Personas asociadas a su organización e identificadas en GenStudio for Performance Marketing |
| Periodo de tiempo | El trimestre, la temporada, el año u otra unidad de tiempo definida por la organización durante la cual la experiencia publicitaria está activa |
| Región | Región geográfica en la que se inicia la experiencia |
| Idioma | Idiomas para los que se utiliza la experiencia publicitaria |
| Keywords | Palabras clave definidas por el usuario que facilitan la búsqueda y la categorización de la experiencia publicitaria |

Después de combinar o seleccionar tu experiencia, haz clic en **[!UICONTROL Siguiente]** para confirmar la configuración de Meta.

## Paso 4: Confirmar la configuración de la cuenta de Meta

Después de preparar las experiencias publicitarias, debe confirmar la información de la cuenta de Meta. La vista _Meta ad setup_ se ha rellenado con opciones que se derivan de las cuentas de Meta configuradas.

| Detalle | Descripción |
|------------|-------------|
| Cuentas | Cuentas de Meta que se han conectado a GenStudio for Performance Marketing |
| Página de Facebook | Página de Facebook donde se publica la experiencia |
| Cuenta de Instagram | Cuentas de Instagram conectadas a GenStudio for Performance Marketing |
| Campañas | Campañas de Meta a las que pertenece la experiencia publicitaria. |
| Conjuntos de anuncios | Meta y conjuntos a los que pertenece la experiencia de anuncio activado. La configuración determina las ubicaciones finales del anuncio. |

### Crear un nuevo conjunto de anuncios

Puede crear un nuevo conjunto de anuncios durante la configuración de la plataforma clonando un conjunto de anuncios existente durante la configuración de la plataforma. Los conjuntos de anuncios de Meta definen el momento, los detalles de canal y la audiencia de un anuncio específico. Una campaña de Meta puede contener varios conjuntos de anuncios, pero un conjunto de anuncios está asociado exclusivamente a una campaña.

**Para crear un nuevo conjunto de anuncios**:

1. Seleccione una campaña en el menú desplegable _campañas de Meta_.

   La campaña seleccionada determina los conjuntos de anuncios disponibles como opciones en el menú desplegable _Conjuntos de anuncios_.

1. Haga clic en **[!UICONTROL + Crear nuevo conjunto de anuncios]**.

   Se abre la ventana emergente _Crear nuevo conjunto de anuncios_, que identifica la campaña de Meta en la que se crea el nuevo conjunto de anuncios.

1. Seleccione el conjunto de anuncios que desea clonar en el menú desplegable _Usar configuración de_.

   GenStudio for Performance Marketing asigna un nombre de conjunto de anuncios predeterminado adjuntando `- Copy` al nombre del conjunto de anuncios seleccionado.

1. (Opcional, pero recomendada) Escriba un nombre de anuncio único en el campo **[!UICONTROL Nuevo nombre del conjunto de anuncios]** para reemplazar el valor predeterminado.

1. Haga clic en **[!UICONTROL Crear conjunto de anuncios]**.

   Ha vuelto a la vista _Configuración de plataforma_, donde se preseleccionó el nuevo conjunto de anuncios. Aparece un mensaje de éxito que incluye un vínculo al conjunto de anuncios en el Administrador de Meta Ads. Este conjunto de anuncios está disponible para futuras activaciones.

>[!NOTE]
>
>Si el conjunto de anuncios se crea correctamente pero no se pudo guardar el nombre del conjunto de anuncios, el conjunto de anuncios se guarda en el Administrador de Meta Ads con su nombre predeterminado (_nombre original del conjunto de anuncios - Copiar_).

### ID de seguimiento

Los ID de seguimiento (nombre del anuncio) proporcionan un mecanismo para recopilar métricas vinculadas al rendimiento de la experiencia. Introduzca el nombre del anuncio en este campo.

Haz clic en **[!UICONTROL Siguiente]** en la esquina superior derecha para obtener una vista previa de la experiencia publicitaria y finalizar la activación.

## Paso 5: Previsualizar y activar el anuncio

La página _Revisar_ muestra su experiencia publicitaria tal y como se ha ensamblado en la _Configuración de experiencias_ y proporciona una última oportunidad para ver y editar su experiencia. Haga clic en **[!UICONTROL Editar sección]** junto a la etiqueta _Configuración de la experiencia_ para realizar los cambios. También puede hacer clic en **[!UICONTROL Atrás]** en la esquina superior derecha para regresar a la página _Configuración de la experiencia_.

### Paso 6: Completar la activación de la experiencia publicitaria

1. Haga clic en **[!UICONTROL Publicar]**.

   La experiencia completa con anuncios de Meta y sus metadatos asociados se insertan directamente en el conjunto de anuncios seleccionado de Meta Ads Manager. Las experiencias se envían al administrador de Meta Ads en un estado inactivo. Desde Meta Ads Manager, puede administrar los pasos finales de implementación de la experiencia publicitaria y la campaña de Meta.

1. [Inicie sesión en el Administrador de Meta Ads](https://adsmanager.facebook.com/) para revisar su experiencia publicitaria y finalizar la publicación en canales específicos de Meta.
