---
title: Flujo de trabajo de activación
description: Obtenga información acerca del flujo de trabajo de activación para experiencias publicitarias.
feature: Experiences
source-git-commit: c3b8419deccd24cd565627fcb3f7d6376860e84a
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---

# Flujo de trabajo de activación

_[!DNL Activate]_admite la activación de experiencias de anuncio en formatos específicos de canal, como una experiencia de anuncio Meta.

Una experiencia de GenStudio for Performance Marketing es un componente de campaña de marketing, como un anuncio, que se adapta a una audiencia específica en un canal de publicidad de pago o correo electrónico. Las experiencias publicitarias contienen tres componentes principales:

* **Recursos multimedia**: Los recursos multimedia son las imágenes (GIF, PNG, JPEG) incluidas en su experiencia publicitaria. Actualmente, Activation admite imágenes estáticas.
Para seleccionar un recurso de imagen para la experiencia publicitaria, es necesario elegir una relación de aspecto adecuada. Las relaciones de aspecto definen la relación proporcional entre la anchura y la altura de una imagen y son cruciales para la eficacia de las ubicaciones de anuncios. Los canales de medios de pago especifican cuidadosamente las relaciones de aspecto válidas para cada ubicación de publicidad en su plataforma. Al añadir recursos de imagen a la activación, debe seleccionar la relación de aspecto en función de las ubicaciones de los anuncios finales para su experiencia. Los tipos de archivo están restringidos a JPEG, PNG y GIF.

* **Texto**: el texto incluye todas las formas de texto incluidas en el anuncio, incluidos los titulares, el texto independiente y los elementos de llamada a la acción.

* **Metadatos**: atributos definidos por el usuario que puede asignar al contenido. Los metadatos mejoran el análisis, el filtrado y el seguimiento del rendimiento. Normalmente no es visible para los usuarios.

La creación de una activación implica perfeccionar cada uno de estos componentes de anuncio para una ubicación de canal y una campaña de marketing designadas. GenStudio for Performance Marketing admite la activación de una experiencia en un canal de pago.

## Fases de flujo de trabajo

Aunque los requisitos de ubicación únicos definen cada canal de pago, todas las activaciones de publicidad comparten los mismos pasos de alto nivel. La activación de una experiencia en cualquier canal de pago tiene tres fases principales:

* **Conecte GenStudio for Performance Marketing a su canal de destino**. Un administrador del sistema de GenStudio debe conectar las cuentas de canal para poder activar una experiencia.

* **Prepare su experiencia para la activación**. La preparación incluye la selección de los recursos de medios en la proporción de aspecto adecuada para la ubicación de publicidad específica y la asignación de texto a los elementos de llamada a la acción y a la copia del cuerpo. También puede agregar metadatos informativos que ayuden a los usuarios a buscar la experiencia después de la activación. Cada ubicación de canal de publicidad especifica relaciones de aspecto válidas para los recursos visuales incluidos en la ubicación.

* **Revise y publique su experiencia en el canal de destino**.  Use el panel _Vista previa_ en el flujo de trabajo de creación de activación para evaluar la elección de la ubicación del anuncio y los elementos de texto antes de finalizar la activación. La revisión final previa a la publicación se realizará en la aplicación de administración de anuncios del canal de destino. Por ejemplo, después de activar una experiencia de Meta Ads en GenStudio for Performance Marketing, debe iniciar sesión en el Administrador de Meta Ads, revisar su experiencia publicitaria y, a continuación, seleccionar sus atributos específicos antes de publicarla.

Una vez que una experiencia está activa en su canal de anuncios de destino, _[!DNL Insights]_puede realizar el seguimiento y analizar sus datos de rendimiento.

## Canales admitidos

Cada canal de medios de pago tiene un flujo de trabajo de activación único. Seleccione el canal de pago para las directrices de activación:

* [Meta](activate-meta-ad.md)
