---
title: Integración de Workfront Proof con revisión y aprobaciones
description: Integración de Workfront Proof con Adobe GenStudio for Performance Marketing.
feature: Content Review, Content Management
source-git-commit: f8508ee9440714137141e933cfe0f5761a510c7a
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Integración de Workfront Proof con GenStudio for Performance Marketing

La integración con Workfront Proof mejora el ciclo de vida de revisión y aprobación de GenStudio for Performance Marketing con funciones avanzadas, incluidas plantillas de aprobación, flujos de trabajo de varias fases y la capacidad de [comparar versiones de prueba](https://experienceleague.adobe.com/es/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs). Este control de versiones estructurado garantiza la transparencia, la responsabilidad y la colaboración optimizada a lo largo del ciclo de vida de la revisión de contenido.

>[!BEGINSHADEBOX]

**Requisitos previos**:

Instale la [extensión de Adobe Workfront Web Viewer](https://experienceleague.adobe.com/es/docs/workfront/using/review-and-approve-work/proofing/review-proofs-in-workfront/review-a-proof/review-proof-in-web-viewer-extension)

>[!ENDSHADEBOX]

[!DNL Proofing Viewer] de Workfront Proof es un área de trabajo enriquecida para ver, comentar y comparar pruebas. Desde [!DNL Proofing Viewer], puede

* Comparar distintas versiones del contenido
* Agregar comentarios y dibujar marcas en una prueba
* Aprobar la prueba

[!DNL Proofing Viewer] se carga cuando hace clic en la URL de prueba en el correo electrónico de su solicitud de aprobación o en la notificación interna del producto. Se abre la vista [!DNL Proofing Viewer] _Mi nueva aprobación_. Desde esta vista, puede revisar el contenido y proporcionar comentarios mediante las herramientas de anotación principales de [!DNL Proofing Viewer].

Para salir de [!DNL Proofing Viewer], haga clic en **[!UICONTROL Volver a GenStudio]**.

## Genstudio para Performance Marketing y Workfront Proof: Comparación de características

La siguiente tabla compara las funciones estándar de revisión y aprobación de GenStudio for Performance Marketing con las funciones más avanzadas disponibles a través de la integración de Workfront Proof.

| Función        | GenStudio for Performance Marketing                                                                 | Workfront Proof                                                                 |
|-------------------------------|------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| **Ciclo de vida de borrador/prueba**        | El contenido del borrador caduca tras la publicación. | Cadenas de aprobación de varias fases y basadas en funciones con registros persistentes y con marca de tiempo.<br> Todas las versiones se conservan indefinidamente. |
| **Comentarios**                | Los comentarios están vinculados al ID de borrador y se descartan después de la publicación.                                           | Los comentarios y anotaciones persistentes se conservan para la auditoría y el cumplimiento.     |
| **Versiones**           | Los borradores se tratan como instancias únicas.<br>No hay comparación en paralelo.                                      | Control de versiones completo con herramientas de comparación de superposiciones y en paralelo.        |
| **Administración de proyectos** | Administración de campañas básica. | Administración completa del ciclo de vida de la campaña, incluidas la personalización, las plantillas, la creación de informes y las auditorías detalladas. |

### Licencias y funciones de usuario

Las licencias identifican el conjunto de derechos de usuario dentro de un producto. Workfront Proof proporciona más tipos de licencia o funciones de usuario que GenStudio for Performance Marketing. [Resumen de funciones de revisión](https://experienceleague.adobe.com/es/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles) presenta las funciones de usuario asociadas con el flujo de trabajo de revisión y aprobación de Workfront Proof.

| Licencia de GenStudio for Performance Marketing       | Licencia de Workfront                 | Descripción                                                                                                                                                      |
|---------------------------------------------------|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| GenStudio System Manager                          | Administrador de Workfront/Usuario avanzado | Acceso completo a las funciones de GenStudio Performance Marketing, como la administración de marca, personalidad y productos. Gestiona los flujos de trabajo y la configuración. Crea plantillas de aprobación. |
| Creador y editor de contenido (licencia de usuario avanzado)   | Creador de revisión (licencia estándar)  | Genera y envía borradores de contenido. En el Visor de pruebas, carga los recursos e inicia las pruebas. Requiere una licencia de Workfront Proof.                              |
| Revisor/aprobador (licencia de colaborador)        | Revisor/Aprobador                 | Participa en revisiones de varias fases, agrega comentarios y aprueba o rechaza contenido.                                                                             |

Los administradores del sistema de Adobe administran el aprovisionamiento de usuarios y las autorizaciones para ambos productos en Adobe Admin Console.

>[!NOTE]
>
> Workfront Proof proporciona [funciones de usuario adicionales](https://experienceleague.adobe.com/es/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles). No todos los roles son visibles dentro de Performance Marketing. Sin embargo, el sistema respeta cualquier función establecida dentro de una plantilla de Workfront Proof.

### Borradores y pruebas

Workfront [!DNL Proofing Viewer] amplía el proceso básico de revisión y aprobación de GenStudio for Performance Marketing con características de revisión y aprobación más estructuradas. Las pruebas revisadas en esta integración se limitan a los formatos admitidos por GenStudio for Performance Marketing.

### Control de versiones

GenStudio for Performance Marketing no admite plantillas de aprobación, pero Workfront Proof sí. Las capacidades de versiones de Proof mejoran significativamente el proceso de revisión y aprobación de contenido de GenStudio. Cada envío del flujo de trabajo de prueba se trata como una versión distinta del borrador de contenido o _prueba_. Las pruebas se guardan automáticamente y se pueden comparar en paralelo con iteraciones anteriores. Las partes interesadas pueden realizar un seguimiento de los cambios, proporcionar información precisa y mantener la alineación a lo largo del ciclo de revisión. Proof conserva un historial completo de todos los comentarios, decisiones y versiones, lo que respalda la preparación de la auditoría y los requisitos de cumplimiento. Cada versión también admite flujos de trabajo de aprobación basados en funciones y de varias etapas, con cada acción (aprobación, rechazo o comentario) claramente registrada y con marca de tiempo.

### Plantillas de aprobación

Las plantillas de aprobación de Workfront Proof proporcionan pasos con formato previo que pueden optimizar el flujo de trabajo de aprobación de pruebas. Estas plantillas incluyen revisores y aprobadores seleccionados, funciones de prueba y plazos, lo que garantiza la coherencia y la eficacia. Los creadores de contenido que inicien una revisión pueden seleccionar entre un conjunto de plantillas predefinidas para flujos de trabajo de aprobación monofásicos y multifásicos.

Cada fase de la plantilla de flujo de trabajo identifica los revisores asignados. Todas las actualizaciones de estado y los comentarios del flujo de trabajo de Workfront Proof son visibles en el visualizador de pruebas, lo que mejora la transparencia y la colaboración.

Las plantillas de aprobación admiten aprobaciones de varias etapas, que apoyan la coordinación de los exámenes de diferentes grupos de partes interesadas.

### Comentarios

Los revisores pueden hacer clic directamente en áreas específicas de la prueba para dejar comentarios precisos y contextuales. Todos los comentarios se marcan con la hora y se guardan como parte del historial de versiones de la prueba. El historial de comentarios no está disponible en GenStudio for Performance Marketing.

Puede [comparar dos versiones de una revisión](https://experienceleague.adobe.com/es/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs) para evaluar comentarios y contenido de revisión.

## Notificaciones y recordatorios

Los revisores y aprobadores reciben notificaciones por correo electrónico cuando hay una nueva prueba disponible para su revisión o cuando una revisión en curso ha cambiado de estado.
[Las notificaciones y los recordatorios de prueba](https://experienceleague.adobe.com/es/docs/workfront/using/workfront-proof/proof-notifications-and-reminders/proof-notifications-and-reminders/proof-notifications-and-reminders) incluyen un vínculo personalizado a la prueba, detalles sobre la prueba y su progreso en el proceso de aprobación e información sobre las versiones.
