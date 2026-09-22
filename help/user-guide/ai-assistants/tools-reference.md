---
title: Referencia de herramientas del asistente de IA
description: Obtenga información acerca de las herramientas de perspectivas, crear, activar y recibir comentarios que un asistente de IA puede usar con [!DNL GenStudio for Performance Marketing].
role: User
source-git-commit: 6fb7ddb7549ea6bcd66b6139fbde9ebe12ddaa22
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 15%
---

# Referencia de herramientas del asistente de IA

Esta referencia describe las herramientas que un asistente de IA conectado puede utilizar con [!DNL GenStudio for Performance Marketing]. La lista de herramientas disponibles depende de la configuración de su organización.

Pregunte al asistente de IA a qué herramientas puede acceder antes de iniciar un flujo de trabajo.

## Áreas de funcionalidad

| Área | Función | Comportamiento |
|---|---|---|
| Perspectivas | Consulte el rendimiento de los medios de pago y recupere las recomendaciones creativas. | Solo lectura. |
| Crear | Organice los borradores a partir de plantillas rápidas o recomendaciones de perspectivas y luego administre la revisión. | Leer y escribir. Crea documentos en Creative Cloud. |
| Activar | Resuelva un objetivo de publicación y publique una experiencia aprobada. | Escribir y destruir. Puede publicar un anuncio en directo e incurrir en gastos publicitarios. |
| Comentarios | Enviar comentarios sobre el producto al equipo [!DNL GenStudio for Performance Marketing]. | Escriba. |

La mayoría de las herramientas de Insights cubren `meta`, `linkedin` y `innovid`. Las herramientas de métricas de conversión cubren `meta` y `linkedin`.

Create admite `meta`, `linkedin`, `display`, `tiktok` y `youtube`. Activate admite `META`, `LINKEDIN` y `GOOGLECM360`.

## Herramientas de perspectivas

### get_insights_capability

Devuelve las métricas de conversión personalizadas, las operaciones y los canales de Insights habilitados para su organización. Utilice esta herramienta primero cuando la disponibilidad no sea clara.

Esta herramienta devuelve metadatos de capacidad, no valores de campaña, publicidad o métrica.

### get_insights_summary

Devuelve las métricas y tendencias de rendimiento de titular de un canal en un intervalo de fechas seleccionado.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channel` | Sí | `meta`, `linkedin` o `innovid`. |
| `startDate` | No | Fecha de inicio en formato `YYYY-MM-DD`. El valor predeterminado es hace 30 días. |
| `endDate` | No | Fecha de finalización en formato `YYYY-MM-DD`. El valor predeterminado es hoy. |
| `metrics` | No | Métricas para crear gráficos, como `spend`, `ctr`, `cpc`, `cpm`, `impressions`, `clicks` o `conversions`. |

### list_insights_campaigns

Devuelve una tabla ordenable de métricas de rendimiento de campaña y una fila de totales.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channel` | Sí | `meta`, `linkedin` o `innovid`. |
| `startDate`, `endDate` | No | Intervalo de fecha en formato `YYYY-MM-DD`. El valor predeterminado es los últimos 30 días. |
| `search` | No | Filtro de nombre de campaña. |
| `sortBy` | No | Ordenar campos, como `spend`, `impressions`, `clicks`, `ctr`, `cpc`, `cpm` o `name`. |
| `limit`, `offset` | No | Tamaño de página y desplazamiento de paginación. |

### list_insights_ads

Devuelve el rendimiento a nivel de anuncio. Utilice el modo de exploración predeterminado para una tabla ordenable o un modo de nivel para anuncios de alto y bajo rendimiento.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channel` | Sí | `meta`, `linkedin` o `innovid`. |
| `tier` | No | `all`, `high` o `low`. El valor predeterminado es `all`. |
| `mainMetric` | Condicional | Se requiere una métrica de clasificación para el modo de nivel `high` o `low`. |
| `campaigns` | No | Identificadores de campaña utilizados para limitar el resultado. |
| `search` | No | Filtro de nombre de anuncio. |
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
| `ads` | Sí | Anuncios para explicar, incluidos los identificadores devueltos por `list_insights_ads`. |
| `mainMetric` | Sí | La métrica utilizada para clasificar los anuncios. |
| `campaigns` | No | Identificadores de campaña utilizados para definir la población de comparación. |
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
| `tagSource` | No | `ad_tags` o `campaign_tags`. |
| `sortBy` | No | Métrica utilizada para ordenar el resultado. |
| `search` | No | Filtro de valor de etiqueta. |
| `startDate`, `endDate` | No | Intervalo de fecha en formato `YYYY-MM-DD`. |

### get_insights_custom_metrics

Devuelve las métricas de conversión personalizadas configuradas para su organización. Úselo antes de `get_insights_conversion_metrics`.

Esta herramienta devuelve identificadores de métricas, no valores de métricas.

### get_insights_conversion_metrics

Devuelve los valores y tendencias de las métricas de conversión configuradas para Meta y LinkedIn.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channels` | No | Canal de conversión admitido. El valor predeterminado es `meta`. |
| `metrics` | No | Identificadores de métrica devueltos por `get_insights_custom_metrics`. |
| `campaigns` | No | Identificadores de campaña utilizados para limitar el resultado. |
| `startDate`, `endDate` | No | Intervalo de fecha en formato `YYYY-MM-DD`. |

### get_insights_recommendations

Devuelve los cambios creativos propuestos basados en los datos de rendimiento de su organización. Una solicitud no puede devolver ninguna recomendación cuando el ámbito seleccionado no contiene anuncios aptos.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channels` | Sí | Uno o más canales admitidos. |
| `campaigns` | No | Identificadores de campaña utilizados para limitar el resultado. |
| `search` | No | Filtro de nombre de campaña. |
| `recommendationId` | No | Identificador utilizado para recuperar una recomendación en detalle. |
| `limit`, `offset` | No | Tamaño de página y desplazamiento de paginación. |

## Crear herramientas

Cree herramientas para montar borradores a partir de plantillas de Adobe Express y administrar la revisión antes de que una experiencia esté lista para activarse.

### list_express_templates

Enumera las plantillas Express disponibles con filtrado y recuentos de facetas.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channel` | No | `meta`, `display`, `linkedin`, `tiktok`, `youtube` o `__unspecified__`. |
| `query` | No | Término de búsqueda para plantillas. |
| `aspectRatios`, `keywords`, `languages`, `mediaFormat`, `regions`, `timeframes` | No | Filtros de faceta de plantilla. |
| `sortBy`, `order` | No | Ordenar campo y orden. |
| `limit`, `offset` | No | Tamaño de página y desplazamiento de paginación. |

### describe_express_template

Devuelve los campos de texto editables y las ubicaciones de imágenes en una plantilla.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `templateId` | Sí | Identificador de plantilla expreso. |

### list_cta_options

Devuelve los valores de call-to-action permitidos para un canal.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channel` | Sí | `linkedin`, `meta`, `display`, `tiktok` o `youtube`. |

### create_draft

Crea un borrador editable a partir de una plantilla Express con una o más experiencias.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `templateId` | Sí | Identificador de plantilla expreso. |
| `prompt` | Sí | Instrucciones breves y de copia de Creative almacenadas con el borrador. |
| `experiences` | Sí | Anulaciones de canales, campos de contenido y campos de plantilla opcionales para cada experiencia. |
| `name` | No | Nombre del documento. |

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
| `emails` | Sí | Una o más direcciones de correo electrónico de colaborador. |
| `role` | Sí | `editor` o `viewer`. |
| `message` | No | Mensaje de invitación. |

### request_draft_approval

Envía un borrador a una o varias personas para su aprobación.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `draftId` | Sí | Identificador del borrador del recurso. |
| `emails` | Sí | Una o más direcciones de correo electrónico del revisor. |

### list_experience

Devuelve experiencias aprobadas y publicadas listas para activarse. Los borradores no se incluyen.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `channel` | No | Filtro de canal de experiencia. |
| `createdByMe` | No | Limita los resultados a las experiencias creadas por el usuario actual. |
| `campaignNames` | No | Filtros de nombre de campaña exactos. |
| `creatorEmail` | No | Filtro de correo electrónico del creador. |
| `createdAtFrom`, `createdAtTo` | No | Límites de fecha de creación. |
| `language` | No | Etiqueta de idioma BCP 47. |
| `limit`, `cursor` | No | Tamaño de página y cursor de paginación. |

## Activar herramientas

Active las herramientas para resolver un destinatario de medios de pago y publicar una experiencia aprobada. La publicación no es reversible a través de estas herramientas y podría incurrir en gastos de publicidad.

### configure_activation_target

Resuelve y valida la cuenta de medios de pago, la campaña, el conjunto de anuncios y la página de Facebook cuando es necesario.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `platform` | Sí | `META`, `LINKEDIN` o `GOOGLECM360`. |
| `platformAccountId` | No | Identificador de cuenta de medios de pago. Omítalo para descubrir cuentas. |
| `campaignId` | No | Identificador de campaña para Meta o LinkedIn. |
| `adsetId` | No | Conjunto de anuncios de Meta o identificador de campaña de LinkedIn. |
| `pageId` | No | Identificador de página de Facebook de Meta. |

### create_activation

Publica un anuncio activo de una sola imagen a partir de una experiencia aprobada y un destino validado.

| Parámetro | Requerido | Descripción |
|---|---|---|
| `platform` | Sí | `META`, `LINKEDIN` o `GOOGLECM360`. |
| `targetId` | Sí | Destino validado devuelto por `configure_activation_target`. |
| `experienceId` | Sí | Identificador de experiencia aprobado devuelto por `list_experiences`. |
| `assetId` | No | Identificador de variante de una experiencia con varias variantes aptas. |
| `name` | No | Nombre para mostrar de la ubicación del anuncio. |

Llamar a `create_activation` dos veces crea dos anuncios separados en lugar de actualizar el primer anuncio.

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
- **Revise las métricas de conversión:** Llame a `get_insights_custom_metrics` y luego llame a `get_insights_conversion_metrics` con los identificadores de métrica devueltos.
- **Convierte una recomendación en un borrador:** Llama a `get_insights_recommendations` y luego llama a `create_draft_from_recommendation`.
- **Generar a partir de una plantilla:** Llamar a `list_express_templates`, `describe_express_template` y `list_cta_options`, y después llamar a `create_draft`.
- **Publicar una experiencia aprobada:** Llamar a `list_experiences`, luego llamar a `configure_activation_target` y `create_activation`.

## Funciones relacionadas

- [Información general sobre asistentes de IA](overview.md)
- [Conectar un asistente de IA](connect-ai-assistants.md)
- [Uso de asistentes de IA](use-ai-assistants.md)
