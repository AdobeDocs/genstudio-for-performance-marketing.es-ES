---
title: Activación de un anuncio Meta
description: Obtenga información sobre cómo activar una experiencia de publicidad de Meta.
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
source-git-commit: f98a853965ce05420cd178c294b3b4d69500977b
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 2%

---

# Activación de un anuncio Meta

Adobe GenStudio for Performance Marketing admite la activación de anuncios Meta, o creativos, en Instagram y Facebook.

Puede [crear una experiencia Meta](/help/user-guide/create/create-meta-ad.md) en GenStudio for Performance Marketing y seleccionarla para su activación, o construir una nueva experiencia a partir de recursos aprobados en [!DNL Activate].

La activación de un anuncio Meta sigue los [mismos pasos generales](create-activation.md) necesarios para la activación en otros canales de pago. El proceso de activación admite la preparación de su creatividad a partir de experiencias publicitarias para los requisitos específicos de Meta. Después de activar una experiencia Meta o un elemento creativo en GenStudio for Performance Marketing, usa [Meta Ads Manager](https://adsmanager.facebook.com/) para ajustar la experiencia en ubicaciones específicas de Meta ads antes de la publicación final.

## Paso 1: Configuración de las cuentas Meta

Antes de iniciar una activación, [inicia sesión en Meta](https://adsmanager.facebook.com/) para acceder a tu cuenta de administrador de Meta Ads. Confirme que las cuentas de MetaAd conectadas incluyen:

* Página de Facebook
* Meta campaña
* Meta conjunto de anuncios
* Perfil de Instagram (opcional)

Debe tener permiso para publicar contenido en el administrador de metadatos de anuncios.

## Paso 2: Conéctese a sus cuentas Meta

Para que su organización pueda activar experiencias, un administrador del sistema de GenStudio debe conectar sus cuentas Meta a GenStudio for Performance Marketing. Esta conexión permite que los datos fluyan entre GenStudio y herramientas de marketing externas como Meta, lo que permite los procesos de activación.

Ver [Conectarse a Meta Ads](/help/user-guide/connectors/meta-ads.md).

Una vez finalizada la sincronización, puede ver las cuentas añadidas. Las grandes cantidades de datos tardan más en sincronizarse.

## Paso 3: Prepare su experiencia para la activación

Los administradores de sistemas y editores de GenStudio pueden activar las experiencias publicitarias.

**Para preparar tu experiencia para la activación**:

1. En _[!DNL Activate]_, haga clic en **[!UICONTROL Nuevo]**&#x200B;en el mosaico Meta product. Se abre la vista_ Configuración de Creative _.

   La página de configuración de Creative proporciona una ubicación central para preparar la activación del anuncio Meta. La preparación del anuncio incluye estas tres tareas:

1. Asigne un nombre a su experiencia. Después de la activación, puede usar este nombre para buscar esta experiencia en la tabla de _experiencias activadas_.
1. Seleccione recursos de medios. Puede utilizar recursos desde Contenido o cargar recursos externos (por ejemplo, desde OneDrive o Dropbox).
1. [Agregar texto](#add-ad-text).
1. [Agregar metadatos](#assign-metadata).

   El _panel de vista previa_ admite una vista interactiva del texto y los recursos en el contexto de una ubicación de anuncio específica. Utilice el menú desplegable _Seleccionar ubicación_ para cambiar entre las ubicaciones de anuncios compatibles. Las vistas previas proporcionan la oportunidad de finalizar decisiones sobre elementos de publicidad para ubicaciones específicas. Al seleccionar una ubicación en el panel _Vista previa_, solo se ve afectada la vista del anuncio. No se ha guardado su selección de ubicación en el panel _Vista previa_.

### Selección de los recursos multimedia

Utilice la sección _Medios_ para seleccionar al menos un recurso de imagen para incluirlo en su experiencia. Las ubicaciones de anuncios están asociadas con proporciones de aspecto de imagen admitidas, que se enumeran como opciones en el menú desplegable _Ubicaciones_. Este menú muestra las ubicaciones de anuncios compatibles para publicaciones de Facebook o historias de Instagram, organizadas por proporción de aspecto.

Después de la carga, los recursos se guardan en _[!DNL Content]_. El área_ Media _muestra la imagen de forma predeterminada con una relación de aspecto de 1:1. Las relaciones de aspecto alternativas incluyen solo los valores admitidos por el canal de publicidad de pago. Se agrupan por orientación vertical y horizontal. GenStudio for Performance Marketing admite la inclusión de hasta seis relaciones de aspecto por experiencia activada.

**Para cargar un recurso desde el contenido**:

_[!DNL Content]_&#x200B;proporciona una vista central para los recursos y las experiencias aprobados de su organización. Puede enfocar la galería[_[!DNL Content]_](/help/user-guide/content/manage-assets.md) que muestra el inventario de recursos mediante las opciones de menú **[!UICONTROL Buscar]** (lupa) y _Filtrar_.

1. En _[!DNL Activate]_, haga clic en **[!UICONTROL Nuevo]**&#x200B;en el mosaico Meta Ads. Se abre la vista_ Configuración de Creative _.

1. Haga clic en **[!UICONTROL Seleccionar]** y, a continuación, seleccione **[!UICONTROL Seleccionar del contenido]**. Se abre la vista _Seleccionar contenido_, que muestra una galería de recursos de imagen que puede filtrar o buscar.

1. Utilice las herramientas de búsqueda y filtrado de la galería _[!DNL Content]_&#x200B;para seleccionar al menos un recurso para cargar.

1. Haga clic en **[!UICONTROL Usar]** para incluir el recurso seleccionado en el elemento creativo. La ventana _Configuración de Creative_ incluye el recurso en su proporción de aspecto predeterminada en el área _Medios_. El panel _Vista previa_ obtiene una vista previa del recurso en la ubicación del anuncio que admite esta relación de aspecto.

Si la carga no se ha realizado correctamente, se abrirá un mensaje de error informativo que incluye un vínculo al recurso en _[!DNL Content]_.

**Para cargar un recurso externo**:

Puede cargar hasta seis imágenes estáticas externas a la galería _[!DNL Content]_&#x200B;desde Microsoft OneDrive o Dropbox.

1. En _[!DNL Activate]_, haga clic en **[!UICONTROL Nuevo]**&#x200B;en el mosaico Meta. Se abre la ventana_ Configuración de Creative _.

1. En la sección _Medios_, haga clic en **[!UICONTROL Seleccionar]**. Un menú desplegable muestra opciones para _Seleccionar entre el contenido_ o _Cargar_.

1. Haga clic en **[!UICONTROL Cargar]** Se abre la ventana _Agregar proporciones de aspecto_.

1. Para seleccionar imágenes en las relaciones de aspecto admitidas, arrastre y suelte los archivos de imagen en el área de carga de imágenes. También puede examinar el dispositivo en busca de recursos.

1. (Opcional) Para cargar recursos desde su dispositivo, haga clic en **[!UICONTROL Examinar]** y, a continuación, seleccione _Examinar archivos_ o _Examinar carpetas_ para identificar los recursos que se van a cargar.

1. En el área _Agregar detalles_, agregue detalles informativos a los recursos cargados para facilitar la búsqueda y el filtrado en _[!DNL Content]_. Estos detalles se guardan como metadatos.

1. Cuando haya cargado los recursos y asignado los detalles, haga clic en **[!UICONTROL Agregar Assets]** en la parte inferior derecha.

### Añadir texto del anuncio

Utilice la sección _Texto_ de la página _Activar Meta ad_ para agregar texto atractivo y compatible con la marca a los campos de texto requeridos. Texto incluye el texto principal (cuerpo) del anuncio y el texto de call-to-action.

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

Después de ensamblar el elemento creativo, haga clic en **[!UICONTROL Siguiente]** para confirmar la configuración del elemento Meta.

## Paso 4: Confirmar la configuración de la cuenta Meta

Después de preparar su creatividad, debe confirmar la información de su cuenta Meta y asignar un ID de seguimiento a la experiencia publicitaria. La vista _Meta y configuración_ se rellena con opciones que se derivan de las cuentas Meta configuradas.

| Detalle | Descripción |
|------------|-------------|
| Cuentas | Cuentas meta que se han conectado a GenStudio for Performance Marketing |
| Página de Facebook | Página de Facebook donde se publica la experiencia |
| Cuenta de Instagram | Cuentas de Instagram conectadas a GenStudio for Performance Marketing |
| Campañas | Meta campañas a las que pertenece la experiencia publicitaria |
| Conjuntos de anuncios | Conjuntos de metadatos de publicidad a los que pertenece la experiencia de publicidad activada. La configuración determina las ubicaciones finales del anuncio. |

### ID de seguimiento

Los ID de seguimiento (nombre del anuncio) proporcionan un mecanismo para recopilar métricas vinculadas al rendimiento de la experiencia. Introduzca el nombre del anuncio en este campo.

Haz clic en **[!UICONTROL Siguiente]** en la esquina superior derecha para obtener una vista previa de la experiencia publicitaria y finalizar la activación.

## Paso 5: Previsualizar y activar el anuncio

La página _Revisar_ muestra su experiencia publicitaria tal y como aparece en la _configuración de Creative_ y proporciona una última oportunidad para ver y editar su experiencia. Haga clic en **[!UICONTROL Editar sección]** junto a la etiqueta _Configuración de Creative_ para realizar los cambios. También puede hacer clic en **[!UICONTROL Atrás]** en la esquina superior derecha para volver a la página _Configuración de Creative_.

### Paso 6: Completar la activación de la experiencia publicitaria

1. Haga clic en **[!UICONTROL Publicar]**.

   La experiencia completa con anuncios Meta y sus metadatos asociados se insertan directamente en el conjunto de anuncios Meta Ads Manager seleccionado. Las experiencias se envían al administrador de metadatos de anuncios en un estado inactivo. Desde el administrador de Meta Ads, puede administrar los pasos finales de implementación de la experiencia publicitaria y la campaña de Meta.

1. [Inicie sesión en el administrador de Meta Ads](https://adsmanager.facebook.com/) para revisar su experiencia publicitaria y finalizar la publicación en determinados canales Meta.
