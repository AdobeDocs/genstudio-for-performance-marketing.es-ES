---
title: Flujo de trabajo de activación
description: Obtenga información acerca del flujo de trabajo de activación para experiencias publicitarias.
feature: Ad Activation
exl-id: 17e1bade-d52a-4953-a85c-c10d093e73d6
TQID: https://experienceleague.adobe.com/HSwFeL1qCzgFao2Ii64Hx-kaADRnd3dxaswFMzJ7nfA
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: dd48f9df-f2e2-49fe-a918-332a8e240ffe
    internal-label: Channels
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: c8d964aa325aee782c175abf3fce880fb17ae6ca
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 1%
---
# Flujo de trabajo de activación

[!DNL Activate] activa las experiencias publicadas en sus plataformas de publicidad de pago. Una experiencia de GenStudio for Performance Marketing es un componente de campaña de marketing, como un anuncio, que se prepara para una audiencia específica en una plataforma de publicidad de pago. Las experiencias para la activación contienen tres componentes principales:

* **Recursos multimedia**: imágenes o vídeo en su experiencia publicitaria, en tipos de archivo y proporciones de aspecto que varían según la plataforma y el formato.

* **Texto**: todas las formas de texto incluidas en el anuncio, incluidos los titulares, el texto independiente y los elementos de call-to-action.

* **Metadatos**: atributos definidos por el usuario, normalmente no visibles para la audiencia de publicidad, que mejoran el análisis de rendimiento, el filtrado y el seguimiento.

Estos componentes se preparan y aprueban en [!DNL Content] antes de la activación. [!DNL Activate] no crea ni edita recursos, titulares o texto independiente aprobados. Solo aplica la configuración que cada plataforma necesita y luego publica la experiencia.

Una sola tabla de activación puede incluir experiencias para varias plataformas de publicidad de pago y formatos de publicidad.

>[!VIDEO](https://video.tv.adobe.com/v/3503538?learn=on)

## Conectar las cuentas de plataforma

Un administrador del sistema o editor de GenStudio debe conectar las cuentas de publicidad de cada plataforma de publicidad de pago para poder activar una experiencia en esa plataforma. Para ver los pasos de este proceso, consulta [Conectar cuentas de medios pagados](/help/user-guide/connectors/connect-channel.md).

## Iniciar una activación

Inicie una activación desde uno de los dos puntos de entrada:

* **De[!DNL Content]**: filtrar a Experiencias, seleccione una o más experiencias publicadas y haga clic en **[!UICONTROL Activar]** en la barra de acciones superior.

  ![Seleccionar experiencias publicadas en el contenido y hacer clic en Activar para iniciar una activación](./images/content-select-activate.png)

* **Desde[!DNL Activate]**: en la página de aterrizaje [!DNL Activate], haga clic en **[!UICONTROL + Nueva activación]**. Se abrirá la misma galería de Experiencias, donde puede seleccionar experiencias para su activación.

En cualquier caso, busque por nombre de experiencia o filtre por varios canales para encontrar las experiencias que desee.

Si su selección incluye experiencias en formato de visualización, especifique qué plataforma de visualización utilizar: Google Campaign Manager 360, Innovid, Amazon Ads o The Trade Desk. Luego haga clic en **[!UICONTROL Iniciar activación]**. Para otros formatos, como Meta, LinkedIn, TikTok, YouTube y ChatGPT, [!DNL Activate] infiere la plataforma a partir del canal de la experiencia y omite este paso.

[!DNL Activate] genera una tabla de activación con todas las experiencias seleccionadas.

![Una tabla de activación recién generada agrupada en subtablas de Meta y LinkedIn, con cada anuncio marcado requiere atención hasta que se completen sus campos](./images/activation-table.png)

[!DNL Activate] organiza la tabla en subtablas según el formato de anuncio y la plataforma, por ejemplo, imagen única de Meta o imagen única de LinkedIn. Cada fila representa un anuncio. En la mayoría de las plataformas, como LinkedIn, TikTok y las de visualización, una experiencia con varias relaciones de aspecto genera una fila por relación de aspecto; elimine las filas que no necesite. Meta es la excepción. Un anuncio de Meta puede incluir varias relaciones de aspecto dentro de un solo anuncio, por lo que una experiencia de Meta de relación de aspecto múltiple sigue generando solo una fila.

## Administrar la tabla de activación

La tabla de activación se guarda automáticamente como borrador cuando se abre. Puede salir y reanudar el borrador en cualquier momento antes de publicarlo.

Para agregar más experiencias a una tabla de activación que ya ha abierto, haga clic en **[!UICONTROL Agregar más experiencias]** en la parte superior derecha de la tabla. Esto reabre la Galería de experiencias para que pueda seleccionar experiencias adicionales, que [!DNL Activate] agrega a la tabla existente.

**[!UICONTROL Agregar más experiencias]** también le permite activar más de una plataforma de visualización en la misma tabla. Las experiencias con formato de presentación le piden que elija primero una única plataforma de presentación, pero puede hacer clic en **[!UICONTROL Agregar más experiencias]**, seleccionar más experiencias con formato de presentación y elegir una plataforma de presentación diferente de la que ya se encuentra en la tabla. Por ejemplo, puede agregar The Trade Desk ads a una tabla que ya contiene anuncios Innovid.

Una vez que la tabla tenga las experiencias correctas, configure los campos de cada anuncio a continuación.

## Configuración de los detalles de configuración de publicidad y plataforma

Edite campos en línea por fila o seleccione varias filas dentro de la misma tabla de formato y haga clic en **[!UICONTROL Editar detalles]** en la barra de herramientas que aparece para editar masivamente esos campos a la vez.

![Selección de varios anuncios en una tabla de activación para editar detalles por lotes o la configuración de la plataforma](./images/bulk-edit-action-bar.png)

Los recursos, titulares y texto aprobados están bloqueados y no se pueden editar en la tabla de activación, puesto que ya se han revisado y aprobado en [!DNL Content]. Los campos restantes se pueden editar y variar según la plataforma. [!DNL Activate] solo muestra las columnas relevantes para las plataformas y los formatos que seleccionó. Utilice la tabla siguiente como referencia para lo que se puede editar por plataforma.

**Campos editables por plataforma**

| Plataforma | Formatos admitidos | Copia bloqueada | Campos de texto editables | Campos de configuración de plataforma editables |
|---|---|---|---|---|
| Meta | Imagen, vídeo, carrusel | Titular, cuerpo | Descripción, Call-to-action, URL de destino, parámetros de URL, ID de seguimiento | Cuenta de publicidad, Página de Facebook, Perfil de Instagram, Meta Campaign, Meta Ad Set |
| LinkedIn | Una sola imagen, un solo vídeo | Titular, texto introductorio | Descripción, Call-to-action, URL de destino, parámetros de URL, ID de seguimiento | Cuenta de publicidad, Campaña, Conjunto de anuncios |
| Administrador de Google Campaign 360 | Pantalla estática, pantalla de vídeo, HTML5 Zip Display | N/D | ID de seguimiento | Anunciante |
| Amazon Ads | Visualización estática | N/D | ID de seguimiento | Cuenta |
| Innovid | Pantalla estática, HTML5 Zip Display | N/D | ID de seguimiento | Cuenta, Biblioteca de Creative, Nombre del concepto |
| TikTok | Anuncios de vídeo en la fuente | Texto principal | Call-to-action, URL de destino, ID de seguimiento | Cuenta de publicidad, Campaña, Grupo de publicidad |
| YouTube | Shorts en campañas de Google Ads Demand Gen | Descripción | Call-to-action, nombre de la empresa, dirección URL de destino, parámetros de URL, ID de seguimiento | Cuenta, campaña, grupo de publicidad, logotipo |
| ChatGPT | Tarjetas de chat | Título, cuerpo | URL de destino, ID de seguimiento | Cuenta de publicidad de OpenAI, Campaña de OpenAI, Grupo de publicidad de OpenAI |
| La Oficina de Comercio | Visualización estática | N/D | ID de seguimiento | Cuenta, Campaign |

Para configurar los campos de configuración de la plataforma para un grupo de formatos de anuncio, haga clic en **[!UICONTROL Administrar configuración de la plataforma]** y edite los campos en el cuadro de diálogo resultante.

![Cuadro de diálogo Administrar configuración de plataforma para elegir una cuenta, campaña y conjunto de anuncios de Meta](./images/manage-platform-settings.png)

Los campos **[!UICONTROL ID de seguimiento]** están inicialmente en blanco. Un ID de seguimiento es lo mismo que el nombre publicitario o el nombre creativo de la plataforma de publicidad, y la plataforma de publicidad lo utiliza como nombre identificativo del anuncio. Utilice este campo para identificar ese anuncio para la creación de informes y la resolución de problemas. Escriba los valores que desee usar en los campos **[!UICONTROL ID de seguimiento]**.

![Edición de un campo de ID de seguimiento en línea en la tabla de activación](./images/tracking-id-edit.png)

Para cambiar entre los campos **[!UICONTROL ID de seguimiento]** más rápidamente, use estos métodos abreviados de teclado:

* Pulse **Intro** para abrir el campo de edición del **[!UICONTROL identificador de seguimiento]** seleccionado.
* Presione la tecla de flecha **Arriba** o **Abajo** para pasar al campo **[!UICONTROL ID de seguimiento]** anterior o siguiente de esa columna.
* Pulse **Intro** de nuevo para guardar la edición.

## Revise y publique sus experiencias en sus plataformas de publicidad

Confirme que cada fila muestre [!UICONTROL Listo para activar]. [!DNL Activate] marca campos que faltan o no son válidos, llamadas a la acción incompatibles e ID de seguimiento duplicados como [!UICONTROL Necesita atención]. Cuando cada fila esté lista, haga clic en **[!UICONTROL Enviar a plataformas]** y confirme en el cuadro de diálogo de publicación.

![Tabla de activación en la que cada fila muestra Listo para activar y se habilita Enviar a plataformas](./images/ready-to-activate.png)

[!DNL Activate] informa del estado de cada anuncio en tiempo casi real: Pendiente y Enviado a plataformas o Fallido. Si un anuncio falla, pase el ratón sobre su estado para ver el error de la plataforma. Puede reintentar cada anuncio fallido de la tabla a la vez haciendo clic en **[!UICONTROL Intentar de nuevo]**, en lugar de reintentar cada uno de forma individual. Las filas que ya se han enviado a las plataformas están bloqueadas para que no se vuelvan a enviar e incluyen un vínculo profundo al anuncio en el administrador de anuncios nativo de la plataforma de destino. La revisión final previa a la publicación y el lanzamiento de anuncios se realizan en el administrador de anuncios propio de la plataforma de destino: [!DNL Activate] siempre envía los anuncios en un estado inactivo.

![Una tabla de activación que muestra una combinación de los estados Pendiente y Enviado a las plataformas después de publicar](./images/activation-status-pending.png)

Las tablas de activación aparecerán en la página de aterrizaje [!DNL Activate].

## Plataformas compatibles

Cada plataforma de publicidad de pago tiene campos de configuración y requisitos previos específicos. Seleccione la plataforma de publicidad de pago para las directrices de activación:

* [Meta](activate-meta-ad.md)
* [LinkedIn](activate-linkedin-ad.md)
* [Administrador de Google Campaign 360](activate-cm360-ad.md)
* [Amazon Ads](activate-amazon-ad.md)
* [Innovid](activate-innovid-ad.md)
* [TikTok](activate-tiktok-ad.md)
* [YouTube](activate-youtube-ad.md)
* [ChatGPT](activate-chatgpt-ad.md)
* [La Oficina de Comercio](activate-trade-desk-ad.md)
