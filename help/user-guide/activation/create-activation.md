---
title: Flujo de trabajo de activación
description: Obtenga información acerca del flujo de trabajo de activación para experiencias publicitarias.
feature: Ad Activation
exl-id: 17e1bade-d52a-4953-a85c-c10d093e73d6
source-git-commit: 09090a57a0f41c23e8787bfb267e74427d9b7356
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

# Flujo de trabajo de activación

_[!DNL Activate]_admite la activación de experiencias de publicidad en forma de un elemento creativo en formatos específicos de canal, como una experiencia de anuncio Meta o Google Campaign Manager 360.

Una experiencia de GenStudio for Performance Marketing es un componente de campaña de marketing, como un anuncio, que se prepara como un elemento creativo para una audiencia específica en un canal de publicidad de pago o correo electrónico. Los creativos contienen tres componentes principales:

* **Recursos multimedia**: Los recursos multimedia son las imágenes (GIF, PNG, JPEG) incluidas en su experiencia publicitaria. Actualmente, Activation admite imágenes estáticas.

  Para seleccionar un recurso de imagen para la experiencia publicitaria, es necesario elegir una relación de aspecto adecuada. Las relaciones de aspecto definen la relación proporcional entre la anchura y la altura de una imagen y son cruciales para la eficacia de las ubicaciones de anuncios. Los canales de medios de pago especifican cuidadosamente las relaciones de aspecto válidas para cada ubicación de publicidad en su plataforma. Al añadir recursos de imagen a la activación, debe seleccionar la relación de aspecto en función de las ubicaciones de los anuncios finales para su experiencia. Los tipos de archivo están restringidos a JPEG, PNG y GIF.

* **Texto**: el texto incluye todas las formas de texto que se incluyen en el anuncio, incluidos los titulares, el texto principal y los elementos de call-to-action.

* **Metadatos**: atributos definidos por el usuario que puede asignar al contenido. Los metadatos mejoran el análisis, el filtrado y el seguimiento del rendimiento. Normalmente no es visible para los usuarios.

La creación de una activación implica perfeccionar cada uno de estos componentes de anuncio para una ubicación de canal y una campaña de marketing designadas. GenStudio for Performance Marketing admite la activación de una experiencia en un canal de pago.

## Fases de flujo de trabajo

Aunque los requisitos de ubicación únicos definen cada canal de pago, todas las activaciones de publicidad comparten los mismos pasos de alto nivel. La activación de una experiencia en cualquier canal de pago tiene tres fases principales:

* **Conecte GenStudio for Performance Marketing a su canal de destino**. Un administrador del sistema de GenStudio debe conectar las cuentas de canal para poder activar una experiencia.

* **Prepare su experiencia para la activación**. La preparación incluye la selección de los recursos de medios en la relación de aspecto adecuada para la ubicación específica del anuncio y la asignación de texto a los elementos de call-to-action y a la copia de cuerpo. También puede agregar metadatos informativos que ayuden a los usuarios a buscar la experiencia después de la activación. Cada ubicación de canal de publicidad especifica relaciones de aspecto válidas para los recursos visuales incluidos en la ubicación.

  >[!TIP]
  >
  >Puede seleccionar experiencias de publicidad aprobadas directamente desde la galería de experiencias _[!DNL Content]_para prepararse como creativos de Google Campaign Manager 360. Una vez seleccionada una experiencia en la galería_[!DNL Content]_, no podrá editar ni agregar recursos a su elemento creativo.

* **Revise y publique su experiencia en el canal de destino**. Use el panel _Vista previa_ durante la configuración creativa para evaluar la elección de ubicación de anuncios y elementos de texto antes de finalizar la activación. La revisión final previa a la publicación se realizará en la aplicación de administración de anuncios del canal de destino. Por ejemplo, después de activar una experiencia de Meta Ads en GenStudio for Performance Marketing, debe iniciar sesión en el administrador de Meta Ads, revisar su creativo y, a continuación, seleccionar sus atributos específicos antes de publicarlo.

Una vez que un elemento creativo esté activo en su canal de medios pagados de destino, _[!DNL Insights]_podrá realizar el seguimiento y analizar sus datos de rendimiento.

## Canales admitidos

Cada canal de medios de pago tiene un flujo de trabajo de activación único. Seleccione el canal de pago para las directrices de activación:

* [Meta](activate-meta-ad.md)
* [Administrador de Google Campaign 360](activate-cm360-ad.md)
