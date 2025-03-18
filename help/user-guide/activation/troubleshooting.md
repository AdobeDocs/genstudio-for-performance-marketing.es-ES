---
title: Optimizar la activación
description: Aprenda a optimizar las activaciones a los canales de publicidad de pago de terceros.
source-git-commit: a098e053dffe4835a4425252203977dc6ce44713
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# Optimización de activaciones

La activación de una experiencia de publicidad para canales de publicidad de pago implica dos fases principales:

* Preparación de la experiencia para su activación

* Publicación de la experiencia en los administradores de anuncios de canal de pago designados

Las siguientes prácticas recomendadas al crear y activar la experiencia publicitaria pueden ayudar a minimizar las posibles complicaciones o errores durante la entrega a los canales de destino.

## Prácticas recomendadas

Estas son algunas prácticas recomendadas comunes y los errores que pueden evitar.

* **Use direcciones URL de destino válidas y completas**

  Las direcciones URL no válidas pueden almacenar errores en déclencheur. Error de ejemplo: _La dirección URL que ha especificado no se dirige a un sitio web. Introduzca una URL válida e inténtelo de nuevo. (100)_

* **Asegúrese de que la aplicación administra correctamente la caducidad del token**

  Las aplicaciones deben solicitar nuevos tokens según sea necesario. Si es necesario, vuelva a autenticar y obtenga un nuevo token de acceso iniciando sesión de nuevo o actualizando la sesión. Error de muestra: _Error al validar el token de acceso: la sesión se ha invalidado porque el usuario cambió su contraseña o Facebook cambió la sesión por motivos de seguridad. (190)_

* **Revise su conjunto de anuncios y asegúrese de que solo hay un anuncio activo en cada momento**

  Si necesita activar varios Meta Ads, cree conjuntos de anuncios dinámicos de Creative independientes para cada uno. Error de muestra: _El conjunto de anuncios dinámicos de Creative permite como máximo un anuncio activo en él. Los usuarios no pueden crear más de un anuncio en el mismo conjunto de anuncios de Dynamic Creative. (100)_

* **Hacer coincidir el número de reglas aplicadas con la cantidad especificada por la plataforma**

  Los canales de pago esperan que el número de reglas aplicadas coincida con el formato especificado.  Si es necesario, ajuste el número de reglas para que coincidan con el valor que especifica la plataforma. Error de ejemplo: _La fuente de recursos de publicidad tiene reglas de destino X para format: name of format, pero se espera exactamente la regla de destino X para este formato. (100)_

* **Elija una llamada a la acción (CTA) que sea compatible con el objetivo del conjunto de anuncios**

  Las llamadas a acción que son incompatibles con el objetivo de la déclencheur de conjuntos de anuncios de Dynamic Creative generan un error. Error de muestra: _No se admite la llamada a la acción de tipo X para el objetivo Y en el conjunto de anuncios de Dynamic Creative. (100)_

* **Asegúrese de que el límite del conjunto de anuncios de destino admita el número de experiencias publicitarias**

  Confirme que el límite de anuncios del conjunto de anuncios objetivo se adapta a las experiencias de publicidad activadas. Si es necesario, elimine los anuncios innecesarios o inactivos del conjunto de anuncios para que se mantengan dentro de este límite. También puede crear un nuevo conjunto de anuncios para activar anuncios adicionales. Error de muestra: _Ha alcanzado los límites de campaña, conjunto de anuncios o anuncios por cuenta de publicidad. Cada conjunto de anuncios puede contener un máximo de 50 anuncios. Esto incluye anuncios en pausa/inactivos/desactivados. (100)_

* **Asegúrese de que la plataforma admite el tipo de CTA seleccionado**

  Confirme que su experiencia incluye un tipo de CTA compatible. Error de muestra: _(#100) Llamada no válida al tipo de acción (100)_
