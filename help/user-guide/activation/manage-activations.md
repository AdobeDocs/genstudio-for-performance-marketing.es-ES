---
title: Administración de activaciones
description: Obtenga información sobre cómo administrar experiencias activadas con Adobe GenStudio for Performance Marketing.
feature: Ad Activation
exl-id: 7cf340d4-37ab-4906-9aad-088a26db0818
source-git-commit: 9efa42bac9e5623ace963d0de19eeb24467b69d8
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# Administración de activaciones

_[!DNL Activate]_ofrece una vista centralizada del estado de activación de cada canal de publicidad, incluidas las activaciones Publicado (correcto), Fallido (incorrecto) y Publicación (pendiente). La vista_ Experiencias activadas _muestra todas las activaciones de una cuenta de anuncio de canal conectada.

_[!DNL Activate]_organiza las experiencias activadas por canal de publicidad. Haga clic en **[!UICONTROL Ver]**en el mosaico del canal. Se abre la vista de_ experiencias activadas _para el canal seleccionado. Esta vista enumera las experiencias por nombre y las ordena por fecha de activación. Si su organización no ha activado experiencias para ese canal, el mosaico del producto no incluye el botón **[!UICONTROL Ver]**.

## Vista de experiencia activada

Esta vista enumera las activaciones por nombre de experiencia en orden cronológico descendente (primero la más reciente enumerada).

En la tabla siguiente se enumeran los atributos que definen cada experiencia.

| Atributo | Valor |
|------------------|---------------------------------------------------------------------------------------------|
| Nombre de experiencia | Nombre de la experiencia en GenStudio for Performance Marketing<br>Este nombre identifica la experiencia en _[!DNL Content]_ |
| Nombre del anuncio | Nombre del anuncio en el canal de publicidad |
| Fecha de publicación | Fecha en la que se publicó correctamente la experiencia publicitaria<br>Utiliza el formato mes-día-año |
| Publicado por | Nombre del usuario de GenStudio for Performance Marketing que activó la experiencia |
| Regiones | Región geográfica en la que se inicia la experiencia |
| Estado | Estado de la experiencia de publicidad seleccionada<br>Los valores incluyen Error, Publicado y Publicación |

Use **[!UICONTROL Buscar]** (lupa) o desplácese por la lista de experiencias para encontrar una activación por nombre de experiencia.

Haga clic en la activación para abrir una vista enfocada de los detalles de activación.

## Vista de detalles

En la vista _Experiencias activadas_, haga clic en una activación. La vista de solo lectura _Detalles de activación_ captura los detalles que definen una experiencia activada, incluidas las activaciones fallidas. Esta vista incluye información derivada tanto de GenStudio for Performance Marketing como del canal de publicidad.

* **Fecha y hora de publicación**: Fecha y hora de publicación desde el administrador del canal de publicidad
* **ID de anuncio**: ID asignado por el canal de pago y utilizado para el seguimiento. Haga clic en el botón **[!UICONTROL Abrir]** que se encuentra junto a este campo para ver el anuncio publicado en el Administrador de metadatos de anuncios
* **Detalles de Creative**: los recursos de imagen, textos y metadatos seleccionados asignados durante el flujo de trabajo de activación de GenStudio for Performance Marketing
* **Configuración del canal**: Las cuentas de canal de pago utilizadas para activar la experiencia de anuncio

La vista _Detalles_ de una activación fallida incluye el motivo del error.
