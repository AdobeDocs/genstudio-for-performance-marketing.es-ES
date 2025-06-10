---
title: Revisiones y aprobaciones de Adobe GenStudio for Performance Marketing
description: Obtenga información acerca del proceso de revisión y aprobación de GenStudio for Performance Marketing.
level: Beginner
feature: Content Review, Content Management
exl-id: c83f47c0-e8ae-4c54-84b3-c50f67d6b3c2
source-git-commit: 7955796949c17f7cd877b115cba45c58cdd614a7
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# Revisiones y aprobaciones de Adobe GenStudio for Performance Marketing

El flujo de trabajo de revisión y aprobaciones garantiza que todas las partes interesadas, desde equipos creativos hasta expertos legales, puedan revisar y aprobar de forma eficaz los activos y las experiencias de la campaña, incluidos los activos de marca generados por IA.

>[!NOTE]
>
> Esta característica también está disponible como una [integración con Adobe Workfront Proof](/help/user-guide/approvals/proof-integration.md). Esta integración ofrece funcionalidades de prueba en el lienzo de GenStudio for Performance Marketing. Con la integración de Workfront Proof, GenStudio for Performance Marketing obtiene un proceso de revisión más estructurado, transparente y colaborativo, lo que ayuda a los equipos a pasar de Borrador a Final con mayor confianza y claridad.

## Ventajas del flujo de trabajo de revisión y aprobación

* **Compatibilidad con la creación de contenido de IA generativo, iterativo y robusto**. La creación e implementación de contenido alineado con la marca en una organización es un proceso altamente iterativo. Las capacidades generativas de IA de GenStudio for Performance Marketing admiten la creación rápida de cientos de variantes de recursos. Cada revisor puede solicitar varios cambios en un borrador de recurso antes de aprobarlo. Cuantos más revisores haya, mayor será el número de iteraciones potenciales antes de que todas las partes interesadas acuerden una variante final.

* **Soporte para la integridad creativa**. Las aprobaciones salvaguardan la integridad creativa de los activos de su marca al mantener a los creadores de contenido involucrados en el proceso de aprobación. Al involucrar a las partes interesadas creativas (por ejemplo, creadores de contenido y directores creativos) en el proceso de revisión y aprobación, se asegura de que el resultado final se ajuste a su visión y a la identidad de su marca.

* **Cumplimiento de los objetivos de la campaña y los requisitos legales**. El proceso de aprobación ayuda a comprobar que el contenido admite los objetivos de la campaña. Garantiza que todos los materiales de marketing cumplan con las normas legales y reglamentarias, lo que minimiza los riesgos y los posibles problemas legales.

* **Integración con Adobe Workfront Proof**. Los usuarios pueden acceder a las potentes funciones de revisión y aprobación de Workfront Proof desde GenStudio for Performance Marketing. El contenido revisado en GenStudio for Performance Marketing se sincroniza con Workfront Proof y los comentarios de revisión y el estado se conservan. [Aspectos destacados de la integración](/help/user-guide/approvals/proof-integration.md) identifica cómo Proof extiende el flujo de trabajo de aprobación de GenStudio for Performance Marketing.

## Ciclo de vida de revisión y aprobación

Las fases principales del flujo de trabajo de revisión y aprobación incluyen:

* [Solicitar revisión y aprobación del contenido que ha creado](/help/user-guide/approvals/request-review.md). GenStudio for Performance Marketing optimiza el proceso de solicitud de aprobaciones y administración de aprobadores. Las plantillas de aprobación de Workfront Proof pueden simplificar aún más esta tarea.

* [Revisar y editar contenido](/help/user-guide/approvals/review-and-edit.md). Las notificaciones mantienen a los creadores de contenido en el bucle sobre los cambios y las aprobaciones solicitadas. La revisión de los déclencheur de contenido genera un nuevo ciclo de aprobación automático.

* [Aprobar contenido](/help/user-guide/approvals/approve-content.md). Los aprobadores designados marcan el contenido como aprobado o listo para su publicación.

* [Publicar contenido](/help/user-guide/approvals/publish-content.md). Al publicar el contenido aprobado en [!DNL Content], estará disponible para que otros miembros de su organización lo utilicen o hagan referencia a él.

## Acerca de los borradores de contenido

_Borradores_ son versiones preliminares de recursos o experiencias que no han completado el proceso de revisión y aprobación. El estado del borrador indica dónde se encuentra el borrador en el proceso de revisión y aprobación. Un ID de borrador único identifica cada borrador. Esta ID es válida hasta que se apruebe un borrador y se publique en [!DNL Content]. Los comentarios de revisión y las aprobaciones de un borrador están asociados a este ID de borrador individual. No hay versiones para borradores de contenido de GenStudio.

Cuando un borrador completa el proceso de revisión y aprobación y se publica en [!DNL Content], el ID del borrador caduca. GenStudio for Performance Marketing no guarda los comentarios asociados ni el estado de aprobación. El borrador de URL ya no es válido.

El estado del borrador captura el estado del borrador de contenido a medida que se desplaza por el proceso de revisión y aprobación. El editor de contenido de GenStudio for Performance Marketing que creó el recurso en revisión recibe una notificación de cualquier cambio solicitado en el borrador o en las aprobaciones. Los aprobadores cambian el estado del borrador para indicar si necesita una revisión adicional o si se puede aprobar. Todos los aprobadores designados deben aprobar un recurso o una experiencia para que se pueda publicar.

Estados de borrador disponibles:

**Notificado**: el editor de contenido ha iniciado el proceso de revisión y aprobación al notificar a los aprobadores que un borrador está listo para su revisión.
**Necesita trabajo**: indica que uno o más aprobadores han solicitado cambios en el borrador de contenido. El contenido en este estado no se puede guardar en [!DNL Content].
**Aprobado**: todos los aprobadores designados han aprobado el recurso o la experiencia. El editor de contenido ahora puede agregar metadatos al recurso o la experiencia y guardarlos en [!DNL Content].

>[!NOTE]
>
> Los borradores corresponden a _pruebas_ para los usuarios de la integración de Workfront Proof. [Los borradores y las pruebas](/help/user-guide/approvals/proof-integration.md#drafts-and-proofs) difieren en cuanto a persistencia y versiones.

## Funciones de aprobación

_Los revisores_ pueden agregar comentarios, pero no pueden aprobar el contenido. La participación del revisor es útil, pero no esencial. _Los aprobadores_ deben aprobar el contenido para que pueda avanzar en el proceso de aprobación. La integración de Workfront Proof admite una gama más amplia de funciones de usuario.

## Notificaciones

Las notificaciones internas del producto de GenStudio for Performance Marketing actualizan a los aprobadores y editores de contenido en tiempo real de los cambios de estado de los recursos y `@mention` comentarios. Las notificaciones admiten la iteración rápida a través de varios ciclos de revisión, edición y aprobación.

Los editores y aprobadores de contenido pueden registrarse para recibir estas notificaciones en Slack. Ver [Suscribirse a servicios en Experience Cloud](https://experienceleague.adobe.com/es/docs/core-services/interface/services/customer-attributes/subscription).

Las acciones realizadas por los participantes de la aprobación almacenan en déclencheur las notificaciones automáticas internas del producto y las notificaciones por correo electrónico. Al iniciar un proceso de aprobación, los aprobadores designados reciben notificaciones por correo electrónico y dentro del producto. Se le mantiene al tanto de las notificaciones internas del producto y por correo electrónico cada vez que un aprobador agrega `@mention` comentarios o toma una decisión. Las notificaciones incluyen vínculos al borrador de contenido.

Si ha iniciado el proceso de revisión y aprobación de contenido, se le notifican todas las aprobaciones y comentarios de revisión. Sin embargo, a los aprobadores solo se les notifican los comentarios que los incluyen con un `@mention`.
