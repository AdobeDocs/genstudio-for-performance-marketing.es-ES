---
title: Referencia de herramientas del asistente de IA
description: Obtenga información acerca de las herramientas de perspectivas, crear, planificar, activar y recibir comentarios que un asistente de IA puede usar con [!DNL GenStudio for Performance Marketing].
role: User
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 244293cf4f83acbc252f1d5f3495db403ed4a9bb
workflow-type: tm+mt
source-wordcount: '2265'
ht-degree: 13%
---

# Referencia de herramientas del asistente de IA

Esta referencia describe las herramientas que un asistente de IA conectado puede utilizar con [!DNL GenStudio for Performance Marketing]. La lista de herramientas disponibles depende de la configuración de su organización.

Pregunte al asistente de IA a qué herramientas puede acceder antes de iniciar un flujo de trabajo.

## Áreas de funcionalidad

| Área | Función | Comportamiento |
|---|---|---|
| Perspectivas | Consulte el rendimiento de los medios de pago y del correo electrónico y recupere las recomendaciones creativas. | Solo lectura. |
| Crear | Busque recursos, combine borradores de plantillas urgentes o recomendaciones de perspectivas y, a continuación, administre la revisión. | Leer y escribir. Crea documentos en Creative Cloud. |
| Plan | Extraiga los detalles de una campaña de una breve y guárdelos en Workfront Planning. | La extracción es de solo lectura. Al guardar, se crean registros en Workfront Planning y no se pueden revertir automáticamente. |
| Activar | Resuelva un objetivo de publicación y envíe una experiencia aprobada a la plataforma. | Escriba. Los anuncios se envían a la plataforma y se publican en un estado desactivado. Los enciendes por separado. No reversible con estas herramientas. |
| Comentarios | Enviar comentarios sobre el producto al equipo [!DNL GenStudio for Performance Marketing]. | Escriba. |

La mayoría de las herramientas de Insights cubren `meta`, `linkedin` y `innovid`. Las herramientas de valor de métrica cubren `meta` y `linkedin`. Los informes de campañas de correo electrónico abarcan Adobe Journey Optimizer (`ajo`) y Adobe Campaign (`acc`).

Create admite `meta`, `linkedin`, `display`, `tiktok` y `youtube`. Activate admite `META`, `LINKEDIN` y `GOOGLECM360`.

## Herramientas de perspectivas

### get_insights_capability

Devuelve los canales de Insights y las operaciones de creación de informes habilitadas para su organización. Utilice esta herramienta primero cuando la disponibilidad no sea clara. Los canales admitidos son `meta`, `linkedin`, `innovid`, `ajo` y `acc`.

Esta herramienta devuelve metadatos de capacidad, no valores de campaña, publicidad o métrica. Para encontrar las claves de métrica personalizadas de su organización, use `list_connected_channels_and_metrics`.

### list_connected_channels_and_metrics

Devuelve las conexiones activas de Meta, LinkedIn y Google Campaign Manager 360 de su organización, los canales y operaciones de Insights admitidos y las métricas de conversión personalizadas configuradas. Úselo para buscar claves de métricas antes de llamar a `get_insights_metric_values`.

Esta herramienta devuelve claves de métricas, etiquetas y formatos, no valores de métricas. Las conexiones no garantizan la disponibilidad de los datos del historial de informes.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `limit`, `offset` | No | Tamaño de página y desplazamiento de paginación. Omita ambos para devolver el catálogo completo. |

### get_insights_summary

Devuelve las métricas y tendencias de rendimiento de titular de un canal en un intervalo de fechas seleccionado.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channel` | Sí | `meta`, `linkedin` o `innovid`. |
| `startDate` | No | Fecha de inicio en formato `YYYY-MM-DD`. El valor predeterminado es hace 30 días. |
| `endDate` | No | Fecha de finalización en formato `YYYY-MM-DD`. El valor predeterminado es hoy. |
| `metrics` | No | Métricas para el gráfico: `spend`, `ctr`, `cpc`, `cpm`, `cpa`, `impressions`, `clicks`, `conversions`, `videoPlays`, `engagement`, `likes`, `comments` o `shares`. El valor predeterminado es `spend`, `ctr`, `cpc` y `cpm`. |

### list_insights_campaigns

Devuelve una tabla ordenable de métricas de rendimiento de campaña y una fila de totales.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channel` | Sí | `meta`, `linkedin` o `innovid`. |
| `startDate`, `endDate` | No | Intervalo de fecha en formato `YYYY-MM-DD`. El valor predeterminado es los últimos 30 días. |
| `search` | No | Filtro de nombre de campaña. |
| `sortBy` | No | Campo de ordenación: `spend`, `impressions`, `clicks`, `ctr`, `cpc`, `cpm` o `name`. El valor predeterminado es `spend`. Los resultados siempre se ordenan en orden descendente. |
| `limit`, `offset` | No | Tamaño de página y desplazamiento de paginación. El tamaño de página predeterminado es 20. |

### list_insights_email_campaigns

Devuelve una tabla ordenable de campañas de correo electrónico con métricas de entrega y participación para Adobe Journey Optimizer y Adobe Campaign. Para campañas publicitarias, use `list_insights_campaigns`.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channel` | Sí | `ajo` o `acc`. |
| `startDate`, `endDate` | No | Intervalo de fecha en formato `YYYY-MM-DD`. El valor predeterminado son los últimos 30 días antes de la fecha de finalización. |
| `search` | No | Filtro de nombre de campaña. |
| `sortBy` | No | Campo de ordenación: `campaignName`, `emailsNumber`, `emailsDelivered`, `totalClicks`, `openRate`, `ctr`, `ctor`, `bounceRate`, `unsubscribeRate` o `spamComplaintRate`. El valor predeterminado es `emailsDelivered`. Los resultados siempre se ordenan en orden descendente. |
| `limit`, `offset` | No | Tamaño de página y desplazamiento de paginación. |

### list_insights_ads

Devuelve el rendimiento a nivel de anuncio. Utilice el modo de exploración predeterminado para una tabla ordenable o un modo de nivel para anuncios de alto y bajo rendimiento.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channel` | Sí | `meta`, `linkedin` o `innovid`. |
| `tier` | No | `all`, `high` o `low`. El valor predeterminado es `all`. |
| `mainMetric` | No | Métrica de clasificación para el modo de nivel `high` o `low`: `ctr`, `cpc`, `cpm`, `cpa`, `spend`, `impressions` o `clicks`. Se ignora en el modo Examinar. |
| `metrics` | No | Métricas adicionales para informar de cada anuncio en el modo de nivel. |
| `campaigns` | No | Campañas utilizadas para limitar el resultado, hasta 50. Cada campaña incluye `channel`, `accountId` y `campaignId`. |
| `search` | No | Filtro de nombre de anuncio. |
| `sortBy` | No | Campo de ordenación del modo de exploración: `spend`, `impressions`, `clicks`, `ctr`, `cpc`, `cpm` o `name`. El valor predeterminado es `spend`. Los resultados siempre se ordenan en orden descendente. |
| `spendMin`, `spendMax` | No | Límites de gasto totales para cada anuncio. Solo modo de nivel. |
| `includeUnsupported` | No | Incluye anuncios cuyo creativo no se puede procesar. El valor predeterminado es `false`. |
| `startDate`, `endDate` | No | Intervalo de fecha en formato `YYYY-MM-DD`. |
| `limit`, `offset` | No | Tamaño de página y desplazamiento de paginación. |

El modo de nivel devuelve los identificadores de anuncio necesarios para `get_insights_ad_attributes`.

### get_insights_ad_details

Devuelve metadatos creativos para un anuncio, incluidos texto, call to action, recursos y ubicaciones. No devuelve métricas de rendimiento.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channel` | Sí | `meta`, `linkedin` o `innovid`. |
| `accountId` | Sí | Identificador de cuenta de medios de pago. |
| `campaignId` | Sí | Identificador de campaña. |
| `adId` | Sí | Identificador del anuncio. |
| `adgroupId` | No | Identificador del grupo de anuncios cuando el canal utiliza grupos de anuncios. |

### get_insights_ad_attributes

Compara los rasgos creativos de los anuncios seleccionados con el promedio de canal. Utilícelo después de que `list_insights_ads` identifique los anuncios de alto o bajo rendimiento.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `ads` | Sí | Uno a 200 anuncios para explicar. Cada anuncio incluye `channel`, `accountId`, `campaignId` y `adId`, y opcionalmente `adGroupId` y `performanceTier` (`high` o `low`). Use los identificadores devueltos por `list_insights_ads` en el modo de nivel. |
| `mainMetric` | Sí | La métrica utilizada para clasificar los anuncios: `ctr`, `cpc`, `cpm`, `cpa`, `spend`, `impressions` o `clicks`. |
| `campaigns` | No | Campañas utilizadas para definir la población de comparación, hasta 50. Cada campaña incluye `channel`, `accountId` y `campaignId`. |
| `spendMin`, `spendMax` | No | Gasto de límites para la población de comparación. |
| `startDate`, `endDate` | No | Intervalo de fecha en formato `YYYY-MM-DD`. |

### get_insights_tag_categories

Devuelve las categorías de etiquetas disponibles para su organización durante el periodo solicitado. Devuelve nombres de categoría, no métricas de rendimiento.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channels` | Sí | Uno o más canales admitidos. |
| `startDate`, `endDate` | No | Intervalo de fecha en formato `YYYY-MM-DD`. |

### get_insights_ad_tags

Devuelve el rendimiento por valor de etiqueta dentro de una categoría, como producto, región o tema creativo.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channel` | Sí | `meta`, `linkedin` o `innovid`. |
| `tagCategory` | Sí | Una categoría devuelta por `get_insights_tag_categories`. |
| `tagSource` | No | `ad_tags` o `campaign_tags`. El valor predeterminado es `ad_tags`. |
| `sortBy` | No | Campo de ordenación: `adsCount`, `spend`, `impressions`, `clicks`, `conversionCount`, `ctr`, `cpc`, `cpm` o `cpa`. El valor predeterminado es `adsCount`. |
| `search` | No | Filtro de valor de etiqueta. |
| `startDate`, `endDate` | No | Intervalo de fecha en formato `YYYY-MM-DD`. |
| `limit`, `offset` | No | Tamaño de página y desplazamiento de paginación. |

### get_insights_metric_values

Devuelve los valores y las tendencias de las métricas de las que realiza un seguimiento de su organización, como clientes potenciales, suscripciones o retorno de la inversión en publicidad, para Meta y LinkedIn.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channels` | No | `meta`, `linkedin` o ambos. |
| `metrics` | No | `list_connected_channels_and_metrics` devolvió hasta 20 claves de métrica. El valor predeterminado es el conjunto visible predeterminado de su organización. |
| `campaigns` | No | Campañas utilizadas para limitar el resultado, hasta 50. Cada campaña incluye `channel`, `accountId` y `campaignId`. |
| `startDate`, `endDate` | No | Intervalo de fecha en formato `YYYY-MM-DD`. El valor predeterminado es los últimos 30 días. |

### get_insights_recommendations

Devuelve los cambios creativos propuestos basados en los datos de rendimiento de su organización. Una solicitud no puede devolver ninguna recomendación cuando el ámbito seleccionado no contiene anuncios aptos.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channels` | Sí | Uno o más de `meta`, `linkedin` o `innovid`. |
| `campaigns` | No | Campañas utilizadas para limitar el resultado, hasta 50. Cada campaña incluye `channel`, `accountId` y `campaignId`. |
| `search` | No | Filtro de nombre de campaña. |
| `recommendationId` | No | `adUid` de una recomendación, utilizada para recuperarla en detalle. |
| `onlyWithPreview` | No | Excluye las recomendaciones que no tienen una previsualización creativa de ejemplo. El valor predeterminado es `true`. |
| `limit`, `offset` | No | Tamaño de página y desplazamiento de paginación. |

## Crear herramientas

Cree herramientas para buscar recursos, montar borradores a partir de plantillas de Adobe Express y administrar la revisión antes de que una experiencia esté lista para activarse.

### list_express_templates

Enumera las plantillas Express disponibles con filtrado y recuentos de facetas.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channel` | No | `meta`, `display`, `linkedin`, `tiktok`, `youtube` o `__unspecified__`. |
| `query` | No | Término de búsqueda para plantillas. |
| `activatableMimeType`, `aspectRatios`, `externalTemplateSource`, `isHTML5Template`, `keywords`, `languages`, `mediaFormat`, `regions`, `timeframes` | No | Filtros de faceta de plantilla. |
| `sortBy` | No | `modified` o `created`. El valor predeterminado es `modified`. |
| `order` | No | `asc` o `desc`. El valor predeterminado es `desc`. |
| `limit`, `offset` | No | Tamaño de página y desplazamiento de paginación. |

### describe_express_template

Devuelve los campos de texto editables y las ubicaciones de imágenes en una plantilla.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `templateId` | Sí | Identificador de plantilla expreso. |

### list_cta_options

Devuelve los valores de call-to-action permitidos para un canal. Display devuelve una lista vacía porque acepta texto de forma libre.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channel` | Sí | `linkedin`, `meta`, `display`, `tiktok` o `youtube`. |
| `limit`, `offset` | No | Tamaño de página y desplazamiento de paginación. Omita ambos para devolver todas las opciones. |

### search_assets

Busca las imágenes y los vídeos en el contenido de GenStudio. Utilícela para seleccionar recursos existentes para un borrador. Se excluyen los recursos derivados, externos y caducados. Esta herramienta no carga, edita, elimina ni genera recursos y requiere la asignación de derechos de contenido de GenStudio.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `query` | No | Búsqueda de palabras clave o en lenguaje natural en los metadatos de los recursos. |
| `mediaTypes` | No | `image`, `video` o ambos. El valor predeterminado incluye ambos. |
| `aspectRatios` | No | Proporciones de aspecto como `1:1` o `16:9`. Si una proporción no está disponible, la herramienta devuelve las opciones disponibles. |
| `brands`, `campaigns`, `products`, `personas`, `channels` | No | Filtra por nombre. |
| `customMetadata` | No | Hasta 5 campos de metadatos, cada uno con uno o más valores. |
| `uploadedBy` | No | `me` o una dirección de correo electrónico del cargador. |
| `createdAtFrom`, `createdAtTo` | No | Los límites de tiempo de creación están en formato ISO 8601. |
| `aiGenerated` | No | Filtra por estado de generación de IA. |
| `contentCredentials` | No | Filtra por estado de Content Credentials. |
| `limit`, `offset` | No | Tamaño de página y desplazamiento de paginación. |

El resultado incluye referencias de recursos estables para `create_draft` y direcciones URL firmadas de corta duración.

### create_draft

Crea un borrador editable a partir de una plantilla Express con una o más experiencias. Cada llamada a crea un nuevo borrador.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `templateId` | Sí | Identificador de plantilla expreso. |
| `prompt` | Sí | Instrucciones breves y de copia de Creative almacenadas con el borrador. |
| `experiences` | Sí | Una o más experiencias. Consulte la siguiente tabla. |
| `name` | No | Nombre del documento. |
| `allowAssetReuse` | No | Permite reutilizar un recurso seleccionado en varias experiencias. El valor predeterminado es `false`. |

Cada experiencia admite estos campos:

| Campo | Requerido | Descripción |
|---|---|---|
| `channel` | Sí | `linkedin`, `meta`, `display`, `tiktok` o `youtube`. |
| `title` | No | Título de la experiencia. El valor predeterminado es &quot;Concepto *n*&quot;. |
| `headline` | Meta y LinkedIn | Titular principal. |
| `body` | Meta, LinkedIn y TikTok | Copia de cuerpo. Para LinkedIn, este es el texto introductorio. Para TikTok, este es el texto principal. |
| `description` | YouTube | Descripción del anuncio. Opcional para Meta y LinkedIn. |
| `display_url` | Meta y LinkedIn | Mostrar la URL mostrada en el anuncio. |
| `destination_url` | No | Dirección URL a la que está vinculado el anuncio. |
| `cta` | No | Texto de call-to-action de `list_cta_options`. |
| `templateFields` | No | Invalida elementos de plantilla con nombre de `describe_express_template`. Cada anulación establece un texto, una dirección URL de imagen con dimensiones o una dirección URL de vídeo. |
| `assetTemplateFields` | No | Recursos de contenido de `search_assets` para campos de imagen o vídeo en la plantilla. |

Use `list_cta_options` antes de crear un borrador para un canal con valores call-to-action fijos.

### create_draft_from_recommendation

Crea un borrador editable a partir de una recomendación de Insights específica.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channel` | Sí | `meta` o `linkedin`. |
| `adUid` | Sí | Identificador de recomendación devuelto por `get_insights_recommendations`. |
| `prompt` | Sí | Información de Creative basada en la recomendación. |
| `name` | No | Nombre del documento. |

### list_recent_drafts

Enumera los borradores recientes de la plantilla Express con su estado y vínculos.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `limit`, `offset` | No | Tamaño de página y desplazamiento de paginación. |

### get_draft_metadata

Devuelve el nombre del borrador, los canales, el estado de aprobación, los resultados del revisor y el acceso de los colaboradores.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `draftId` | Sí | Identificador del borrador del recurso. |

### share_draft

Otorga a los colaboradores acceso de visualización o edición a un borrador sin solicitar aprobación.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `draftId` | Sí | Identificador del borrador del recurso. |
| `emails` | Sí | Direcciones de correo electrónico de uno a 20 colaboradores. |
| `role` | Sí | `editor` o `viewer`. |
| `message` | No | Mensaje de invitación. |

### request_draft_approval

Envía un borrador a una o varias personas para su aprobación.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `draftId` | Sí | Identificador del borrador del recurso. |
| `emails` | Sí | Direcciones de correo electrónico de uno a 20 revisores. |

### list_experience

Devuelve experiencias aprobadas y publicadas listas para activarse. Los borradores no se incluyen.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channel` | No | `email`, `meta`, `meta_organic`, `display`, `ctv`, `linkedin`, `linkedin_organic`, `tiktok`, `chatgpt` o `youtube`. |
| `createdByMe` | No | Limita los resultados a las experiencias creadas por el usuario actual. |
| `campaignNames` | No | Hasta 5 filtros de nombre de campaña exactos. |
| `creatorEmail` | No | Filtro de correo electrónico del creador. |
| `createdAtFrom`, `createdAtTo` | No | Límites de fecha de creación. |
| `language` | No | Etiqueta de idioma BCP 47. |
| `limit`, `cursor` | No | Tamaño de página (1-50, predeterminado 20) y cursor de paginación. |

## Herramientas de planificación

Las herramientas de planificación convierten un informe de campaña en un borrador de campaña revisable y lo guardan en Workfront Planning.

### extract_campaign_from_brief

Extrae un borrador de campaña revisable de una información de marketing pegada. Esta herramienta no guarda ningún registro. Los hechos y fechas que faltan no se deducen.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `briefText` | Sí | Texto sin formato completo de una campaña, con hasta 100 000 caracteres. No se admiten archivos y vínculos. |

El resultado incluye un borrador de campaña, conclusiones con comillas de compatibilidad, audiencias sugeridas y advertencias.

### create_workfront_campaign

Crea una campaña de Workfront Planning con productos vinculados y perfiles a partir de un borrador que ha revisado y aprobado. Esta herramienta no es idempotente y los registros no se pueden revertir automáticamente. Inspeccione Workfront antes de reintentar una escritura que podría haber tenido éxito.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `campaignDraft` | Sí | El borrador aprobado. Requiere `name`. Los campos opcionales son `description`, `objective`, `keyMessaging`, `startDate`, `endDate` (`YYYY-MM-DD`), `status`, `channels`, `products` y `personas`. |
| `channelSelections` | No | Opciones aprobadas para nombres de canal ambiguos. |
| `entitySelections` | No | Registros de producto y persona aprobados existentes. Use `null` para solicitar un nuevo registro. |
| `createMissingEntities` | No | Crea los productos y los perfiles que ha seleccionado como nuevos. El valor predeterminado es `false`. |

Si un producto, una persona o un canal es ambiguo, la herramienta devuelve opciones para confirmar y no realiza cambios.

## Activar herramientas

Active las herramientas para resolver un destinatario de medios de pago y enviar una experiencia aprobada a la plataforma. Los anuncios se publican en un estado desactivado (Meta en pausa, borrador de LinkedIn, Campaign Manager 360 inactivo), por lo que debe activarlos por separado antes de que se publiquen. El envío de anuncios a la plataforma no es reversible a través de estas herramientas.

### configure_activation_target

Resuelve y valida la cuenta de medios de pago, la campaña, el conjunto de anuncios y la página de Facebook cuando es necesario.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `platform` | Sí | `META`, `LINKEDIN` o `GOOGLECM360`. |
| `platformAccountId` | No | Identificador de cuenta de medios de pago. Omítalo para descubrir cuentas. |
| `campaignId` | No | Identificador de campaña para Meta o LinkedIn. No se usa para Campaign Manager 360. |
| `adsetId` | No | Conjunto de anuncios de Meta o identificador de campaña de LinkedIn. No se usa para Campaign Manager 360. |
| `pageId` | No | Identificador de página de Facebook de Meta. |

Para Campaign Manager 360, solo se requiere la cuenta de publicidad.

### create_activation

Envía una experiencia aprobada a la plataforma como anuncios, utilizando un destinatario validado. Los anuncios se publican en un estado desactivado. Meta crea un anuncio con la primera imagen para cada relación de aspecto. LinkedIn y Campaign Manager 360 crean un anuncio para cada imagen resuelta.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `platform` | Sí | `META`, `LINKEDIN` o `GOOGLECM360`. |
| `targetId` | Sí | Destino validado devuelto por `configure_activation_target`. |
| `experienceId` | Sí | Identificador de experiencia aprobado devuelto por `list_experiences`. |
| `name` | No | Nombre para mostrar de la ubicación del anuncio. El valor predeterminado es el título del anuncio de la experiencia. |

El resultado enumera el número de anuncios creados, en cola y omitidos, con el estado inicial de cada anuncio y un vínculo al mismo en [!DNL GenStudio for Performance Marketing]. Un estado de `PENDING` significa que el trabajo está en cola, no que el anuncio se está entregando.

Llamar a `create_activation` dos veces crea anuncios adicionales en lugar de actualizar los primeros anuncios.

## Herramienta Comentarios

### submit_mcp_feedback

Envía comentarios sobre una herramienta o un flujo de trabajo al equipo [!DNL GenStudio for Performance Marketing].

| Parámetro | Requerido | Descripción |
|---|---|---|
| `category` | Sí | `bug`, `feature_request` o `workflow_friction`. |
| `comment` | Sí | Una descripción concisa de los comentarios. |
| `tags` | No | Etiquetas utilizadas para categorizar los comentarios. |
| `tool_name` | No | La herramienta asociada con los comentarios. |

## Flujos de trabajo comunes

Utilice estas secuencias cuando una herramienta proporcione identificadores o configuración para otra:

- **Diagnosticar un anuncio:** Llamar a `list_insights_ads` en el modo de nivel `high` o `low` y luego llamar a `get_insights_ad_attributes` con la misma métrica de clasificación.
- **Analizar por etiqueta:** Llamar a `get_insights_tag_categories` y después llamar a `get_insights_ad_tags` con una categoría devuelta.
- **Revise las métricas rastreadas:** Llame a `list_connected_channels_and_metrics` y luego llame a `get_insights_metric_values` con las claves de métrica devueltas.
- **Convierte una recomendación en un borrador:** Llama a `get_insights_recommendations` y luego llama a `create_draft_from_recommendation`.
- **Generar a partir de una plantilla:** Llamar a `list_express_templates`, `describe_express_template` y `list_cta_options`, y después llamar a `create_draft`.
- **Generar a partir de recursos existentes:** Llamar a `search_assets` y pasar las referencias de recursos devueltas a `create_draft` en `assetTemplateFields`.
- **Guardar un informe de campaña en Workfront:** Llamar a `extract_campaign_from_brief`, revisar el borrador y después llamar a `create_workfront_campaign`.
- **Envía una experiencia aprobada a una plataforma:** Llama a `list_experiences`, luego llama a `configure_activation_target` y `create_activation`.

## Funciones relacionadas

- [Información general sobre asistentes de IA](overview.md)
- [Conectar un asistente de IA](connect-ai-assistants.md)
- [Uso de asistentes de IA](use-ai-assistants.md)
