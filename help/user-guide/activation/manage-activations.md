---
title: Administrar activaciones
description: Obtenga información sobre cómo administrar experiencias activadas con Adobe GenStudio for Performance Marketing.
feature: Ad Activation
exl-id: 7cf340d4-37ab-4906-9aad-088a26db0818
TQID: https://experienceleague.adobe.com/ird0IiW8L5Axjj2FmEjlUcD1sPaNCNfxj9XNqGfQWiI
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 361
ht-degree: 1%

---

# Administración de activaciones

[!DNL Activate] ofrece una vista centralizada del estado de activación de cada canal de publicidad, incluidas las activaciones Publicado (correcto), Fallido (incorrecto) y Publicación (pendiente). La vista _Experiencias activadas_ muestra todas las activaciones de una cuenta de anuncio de canal conectada.

[!DNL Activate] organiza las experiencias activadas por canal de publicidad. Haga clic en **[!UICONTROL Ver]** en el mosaico del canal. Se abre la vista de _experiencias activadas_ para el canal seleccionado. Esta vista enumera las experiencias por nombre y las ordena por fecha de activación. Si su organización no ha activado experiencias para ese canal, el mosaico del producto no incluye el botón **[!UICONTROL Ver]**.

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
* **ID de anuncio**: ID asignado por el canal de pago y utilizado para el seguimiento. Haga clic en el botón **[!UICONTROL Abrir]** situado junto a este campo para ver el anuncio publicado en el Administrador de Meta Ads
* **Detalles de la experiencia**: los recursos de imagen, los textos y los metadatos seleccionados asignados durante el flujo de trabajo de activación de GenStudio for Performance Marketing
* **Configuración del canal**: Las cuentas de canal de pago utilizadas para activar la experiencia de anuncio

La vista _Detalles_ de una activación fallida incluye el motivo del error.
