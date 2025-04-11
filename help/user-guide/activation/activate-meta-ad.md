---
title: Activar un meta anuncios
description: Aprende a activar un Meta anuncios experiencia.
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
source-git-commit: 8e61fa5c08102c5dd9905e693d7f129105d9f633
workflow-type: tm+mt
source-wordcount: '1372'
ht-degree: 2%

---

# Activar un meta anuncios

Adobe Systems GenStudio for Performance Marketing admite el activación de Meta anuncios, o creatividades, a Instagram y Facebook.

Puede [crear un Meta experiencia](/help/user-guide/create/create-meta-ad.md) en GenStudio para Performance Marketing y seleccionarlo para activación, o construir un nuevo experiencia a partir de activos aprobados en [!DNL Activate].

La activación de un Meta anuncios sigue los [mismos pasos](create-activation.md) generales requeridos para activación a otros canales pagos. El proceso activación ayuda a preparar sus experiencias anuncios para los requisitos específicos de Meta. Después de activar un Meta experiencia, o creativa, en GenStudio para Performance Marketing, usa [Meta Ads Manager](https://adsmanager.facebook.com/) para ajustar el experiencia para ubicaciones específicas de Meta anuncios antes de la publicación final.

## Paso 1: Configura tus cuentas Meta

Antes de iniciar una activación, [inicia sesión en Meta](https://adsmanager.facebook.com/) para acceder a tu cuenta de administrador de Meta Ads. Confirme que sus cuentas de Meta anuncios conectadas incluyen:

* Página de Facebook
* Meta campaña
* Meta conjunto de anuncios
* perfil Instagram (opcional)

Debe tener permiso para entrada contenido al Administrador de metaanuncios.

## Paso 2: Conéctate a tus cuentas Meta

Antes de que su organización pueda activar experiencias, un administrador del sistema GenStudio necesita conectar sus cuentas Meta a GenStudio para Performance Marketing. Esta conexión permite que los datos fluyan entre GenStudio y las herramientas de marketing externas gustar Meta, lo que permite la activación procesos.

Consulte [Conectarse a un meta (Facebook) cuenta](/help/user-guide/connectors/connect-channel.md#meta-ads-connect).

Una vez finalizada la sincronizar, puede vista las cuentas agregadas. Las grandes cantidades de datos tardan más en sincronizar.

## Paso 3: Prepara tu experiencia para activación

Los administradores y editores del sistema GenStudio pueden activar anuncios experiencias.

**Para preparar su experiencia para activación**:

1. En _[!DNL Activate]_, haga clic **[!UICONTROL en Nuevo]**del mosaico Meta producto. Se abre el_ vista de configuración de Creative _.

   La Página de configuración del Creative proporciona una ubicación central para preparar la activación de Meta anuncios. La preparación del anuncios incluye estas tres tareas:

1. Asigne un nombre a su experiencia. Después de activación, puede usar este nombre para búsqueda este experiencia en la _tabla de experiencias_ activadas.
1. Seleccione medios activos. Puede usar activos desde Contenido o cargar activos externos (por ejemplo, desde OneDrive o Dropbox).
1. [añadir texto](#add-ad-text).
1. [añadir metadatos](#assign-metadata).

   El _panel_ Vista previa admite una vista interactiva del texto y la activos en el contexto de un ubicación de los anuncios específico. Utilice el menú desplegable Seleccionar ubicación _para cambiar entre las_ colocaciones anuncios admitidas. Las vistas previas proporcionan la oportunidad para finalizar las decisiones sobre anuncios elementos para ubicaciones específicas. Cuando selecciona un ubicación en el _panel Vista previa_ , solo se ve afectado el vista del anuncios. No se guarda la selección ubicación _del panel Vista previa_ .

### Seleccione su activos medios

Utilice la _sección Medios_ para seleccionar al menos una imagen recurso incluir en su experiencia. Las colocaciones de anuncios están asociadas con proporciones de aspecto de imagen admitidas, que se enumeran como opciones en el _menú desplegable Ubicaciones_ . En este menú se muestran las ubicaciones de anuncios admitidas para anuncios de Facebook o historias de Instagram, organizadas por proporción de aspecto.

Después de cargar, activos se guardan en _[!DNL Content]_. El_&#x200B;área Medios _muestra la imagen de forma predeterminada con una relación de aspecto de 1:1. Las relaciones de aspecto alternativas incluyen solo los valores admitidos por el canal de anuncios paga. Se agrupan por orientación vertical y horizontal. GenStudio para Performance Marketing admite la inclusión de hasta seis relaciones de aspecto por experiencia activado.

**Para cargar un recurso de contenido**:

_[!DNL Content]_proporciona un vista central para las activos y experiencias aprobadas de su organización. Puede enfocar la[_[!DNL Content]_ galería](/help/user-guide/content/manage-assets.md) mostrada inventario de activos utilizando las **[!UICONTROL opciones de menú Search]** (lupa) y _Filtrar_ .

1. En _[!DNL Activate]_, haga clic **[!UICONTROL en Nuevo]**en el mosaico Meta Anuncios. Se abre el_ vista de configuración de Creative _.

1. Haga clic en **[!UICONTROL Seleccionar]** y, a continuación, seleccione **[!UICONTROL Seleccionar del contenido]**. Se abre la _vista Seleccionar contenido_ , que muestra una galería de activos de imágenes que búsqueda o filtra.

1. Utilice _[!DNL Content]_las herramientas de filtro y búsqueda de la galería para seleccionar al menos un recurso para cargar.

1. Haga clic en **[!UICONTROL Usar]** para incluir el recurso seleccionado en el creativa. La _ventana de configuración de Creative_ incluye la recurso en su relación de aspecto predeterminada en el _área Medios_ . El _panel Vista previa_ previsualiza los recurso de la ubicación de los anuncios que admiten esta relación de aspecto.

Si cargar falla, se abre un mensaje de error informativo que incluye un vincular a la recurso en _[!DNL Content]_, .

**Para cargar un recurso** externo:

Puede cargar hasta seis imágenes estáticas externas a la _[!DNL Content]_galería desde Microsoft OneDrive o Dropbox.

1. En _[!DNL Activate]_, haga clic **[!UICONTROL en Nuevo]**en el mosaico Meta. Se abre la_ ventana de configuración _Creative.

1. En la _sección Medios_ , haga clic en **[!UICONTROL Seleccionar]**. Se muestran las opciones que se pueden seleccionar en el contenido _o_ en el que se puede _cargar_.

1. Haga clic en **[!UICONTROL Cargar]** Se abre añadir _ventana de relaciones de_ aspecto.

1. Seleccione imágenes en las relaciones de aspecto admitidas arrastrando y soltando los archivos de imagen en el área de cargar de imagen. Alternativamente, puede explorar su dispositivos en busca de activos.

1. (Opcional) Para cargar activos de su dispositivos, haga clic en **[!UICONTROL Examinar]** y seleccione _Examinar archivos_ o _carpetas_ Examinar para identificar activos para cargar.

1. En el área de detalles _añadir_, agregue detalles informativos a su activos cargada para facilitar la búsqueda y el filtrado en _[!DNL Content]_. Estos detalles se guardan como metadatos.

1. Cuando hayas cargado tu activos y asignado detalles, haz clic en **[!UICONTROL añadir Assets]** en la parte inferior derecha.

### añadir anuncios texto

Utilice la _sección Texto_ de la _Página Activar meta anuncios_ para agregar texto convincente y marca adherente a los campos de texto obligatorios. El texto incluye el texto principal (del cuerpo) para el texto de anuncios y el texto de llamada a acción.

| Campo | Requerido | Carácter límite (máximo) |
|-----------------|---------------------------|---------------------------------|
| Nombre del anuncio | sí | 500 |
| Texto principal | sí | 500 |
| Titular | sí | 255 |
| Descripción | No | 125 |
| Llamada a acción | sí | Sólo opciones del menú desplegable |
| Mostrar URL | No | 1000 |
| Sitio web URL | sí | 1000 |
| Imagen | se requiere al menos uno: |                                 |

_GenStudio requiere el texto_ principal y _el título_ solo para Performance Marketing, no para Meta.

### Asignar metadatos

Los detalles de la experiencia se guardan como metadatos y ayudan a los usuarios a buscar un experiencia. Estos detalles aumentan la visibilidad del experiencia en [!DNL Content]. Utilice estos detalles opcionales definidos por el usuario para identificar el propósito de la experiencia y el contexto o campañas en las que se implementa.

| Detalle | Descripción |
|------------|-------------|
| Campañas | Todas las campañas de GenStudio para Performance Marketing a las que pertenece el experiencia anuncios |
| Marca | Directrices, definidas por usuario o predeterminadas, que permiten a los usuarios establecer directrices marca que capturen la esencia de la identidad de una marca. |
| Productos | Productos asociados con su organización e identificados en GenStudio para Performance Marketing |
| Personas | Personas asociadas con su organización e identificadas en GenStudio para Performance Marketing |
| Período de tiempo | Trimestre, estación, año u otra unidad de tiempo definida por la organización durante la cual el experiencia anuncios está activo |
| Región | área geográfica geográfica en la que se inicia el experiencia |
| Idioma | Idiomas para los que se utiliza el experiencia anuncios |
| Keywords | Palabras clave definidas por el usuario que facilitan la búsqueda y categorización del anuncios experiencia |

Después de armar su creativa, haga clic en **[!UICONTROL Siguiente]** para confirmar su Meta configuración.

## Paso 4: Confirmar la configuración de Meta cuenta

Después de preparar su creativa, debe confirmar su información de Meta cuenta y asignar un ID de seguimiento al experiencia anuncios. El _vista de configuración_ de Meta anuncios se rellena con opciones derivadas de las cuentas de Meta configuradas.

| Detalle | Descripción |
|------------|-------------|
| Cuentas | Cuentas meta que se han conectado a GenStudio para Performance Marketing |
| Página de Facebook | Página de Facebook donde se publica la experiencia |
| cuenta de Instagram | Cuentas de Instagram que se han conectado a GenStudio para Performance Marketing |
| Campañas | Meta campañas a las que pertenece el experiencia anuncios |
| Conjuntos de anuncios | Meta anuncios conjuntos a los que pertenece el experiencia de anuncios activado. La configuración determina las ubicaciones finales de los anuncios. |

### ID de seguimiento

Los ID de seguimiento (nombre anuncios) proporcionan un mecanismo para recopilar métricas vinculadas al rendimiento experiencia. Introduzca el nombre de la anuncios en este campo.

Haga clic **[!UICONTROL en Siguiente]** en la esquina superior derecha para previsualización el anuncios experiencia y finalizar el activación.

## Paso 5: Previsualizar y activar el anuncio

La página _Revisar_ muestra su experiencia publicitaria tal y como aparece en la _configuración de Creative_ y proporciona una última oportunidad para ver y editar su experiencia. Haga clic en **[!UICONTROL Editar sección]** junto a la etiqueta _Configuración de Creative_ para realizar los cambios. También puede hacer clic en **[!UICONTROL Atrás]** en la esquina superior derecha para volver a la página _Configuración de Creative_.

### Todas las aplicaciones activación de su anuncios experiencia

Haga clic en **[!UICONTROL Publicar]**. La experiencia Meta anuncios completa y sus metadatos asociados se insertan directamente en el conjunto de anuncios Administrador de metaanuncios seleccionado. Las experiencias se entregan al Administrador de metaanuncios desactivado. Desde el Administrador de anuncios de meta, puedes administrar los pasos finales de la implementación de la experiencia de anuncios y los campaña metadatos.

### Inicia sesión en Meta Ads Manager para completar activación

Una vez finalizada la activación, debes iniciar sesión en Meta Ads Manager. Desde [Meta Ads Manager](https://adsmanager.facebook.com/), puedes revisar tu experiencia de anuncios y finalizar la publicación en Meta canales específicos.
