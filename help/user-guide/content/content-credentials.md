---
title: Content Credentials para organizaciones
description: Obtenga información sobre cómo aplicar y revisar Content Credentials en GenStudio for Performance Marketing.
level: Intermediate
feature: Content Management, Content Attributes
source-git-commit: 9023c86d45e6fdc8b6ddd0bdedd23eed05e87aae
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 0%

---

# Content Credentials para organizaciones

Descubra cómo las credenciales a prueba de manipulaciones para el contenido que demuestra la autenticidad de la marca y fomenta el cumplimiento están integradas directamente en el flujo de trabajo de marketing.

>[!WARNING]
>
> Actualmente, esta función está en versión beta y solo está disponible para las organizaciones a las que se les ha concedido acceso. Si está interesado, póngase en contacto con el representante del equipo de su cuenta de Adobe o [utilice este vínculo para solicitar la inscripción](https://www.feedbackprogram.adobe.com/c/a/5aWPEOthrDv22Mf9CyekOy?source=qr).


## Introducción a Content Credentials

Una vez activado Content Credentials en Admin Console, los usuarios de GenStudio for Performance Marketing pueden activar Content Credentials para todos los recursos globalmente en la aplicación. Si la opción global para aplicar credenciales está desactivada, los usuarios tienen la opción de aplicar Content Credentials a cada recurso individual.

Una vez publicado el contenido, Content Credentials será visible en plataformas externas, como LinkedIn.

Los administradores son responsables de cargar un certificado X.509 válido en Admin Console. Este paso garantiza que la firma digital de la empresa esté configurada correctamente y lista para su uso en aplicaciones Adobe DX compatibles.

>[!NOTE]
>
>El control de esta configuración podría hacer la transición a Admin Console en el futuro, lo que optimizaría la administración de Content Credentials en todas las aplicaciones y mejoraría la supervisión administrativa.

## ¿Qué es Content Credentials? 

Content Credentials es un tipo de metadatos duradero y estándar en el sector con detalles sobre cómo se creó el contenido e información de identidad sobre los creadores. Content Credentials se puede ver cuando el contenido se publica en línea en plataformas compatibles o con herramientas como [Adobe&#39;s Inspect tool](https://contentauthenticity.adobe.com/inspect) o la [extensión del explorador Adobe Content Authenticity Chrome](https://helpx.adobe.com/es/creative-cloud/help/cai/adobe-content-authenticity-chrome-browser-extension.html).  

La aplicación de Content Credentials puede ayudar a aumentar la transparencia sobre cómo se creó el contenido y puede ayudar a los usuarios a conectarse con su contenido.

[Más información sobre Content Credentials](https://helpx.adobe.com/es/creative-cloud/help/content-credentials.html) en Adobe.

## Firma de marca y seguimiento de recursos

El contenido firmado por una marca desempeña un papel importante en la promoción de la integridad de la marca y la confianza del usuario. Las organizaciones pueden firmar su contenido con una firma de marca única en las aplicaciones de Adobe cuando su certificado está configurado correctamente en Admin Console. Esta garantía de autenticidad se mantiene mediante tecnologías de marca de agua y de huellas digitales invisibles, que ayudan a preservar la durabilidad de la firma a lo largo del ciclo de vida del contenido.

Además de la firma de marcas, las empresas pueden adjuntar ID de recursos directamente a su contenido. Esto facilita un seguimiento eficaz de los recursos, especialmente cuando se comparten o publican en plataformas de medios sociales. Al incorporar los ID de recurso, las organizaciones pueden rastrear el origen y la ruta de distribución de su contenido, mejorando la supervisión y la rendición de cuentas.

## Content Credentials en el flujo de trabajo de marketing

La aplicación de Content Credentials se puede realizar a través del flujo de trabajo de marketing directamente en GenStudio for Performance Marketing, desde la importación y la detección de contenido hasta la activación y exportación. También encontrará credenciales mostradas en el contenido para su revisión en toda la aplicación.

### Importación y descubrimiento

En la Galería de contenido, las credenciales se muestran en los recursos importados.

El distintivo de Content Credential en la esquina superior derecha de la miniatura indica contenido &quot;firmado por la marca&quot;.

![Recurso importado con credenciales](./images/import-discovery1.png)

Al seleccionar contenido firmado, se muestran los metadatos detallados: marca publicada, grabadora, herramienta utilizada, marca de tiempo.

El contenido se puede filtrar por estado de credencial.

![Datos de credencial en un recurso](./images/import-discovery2.png)

### Creación y selección

Los distintivos de Content Credential se muestran en el selector de recursos de lienzo.

Los metadatos de credenciales se conservan a medida que se seleccionan los recursos para las experiencias, a fin de mantener la cadena de procedencia durante la edición.

![insignias de Content Credential en el selector de recursos de lienzo](./images/creation-selection1.png)

### Edición y transformación

Durante las exportaciones de un borrador, los recursos modificados se vuelven a firmar automáticamente y la nueva credencial se vincula al original.

![Datos de credencial de un recurso exportado](./images/edit-and-transformation1.png){width="60%"}

### Revisión y aprobación

En la previsualización Revisar y aprobar, el estado de las credenciales se muestra para los recursos en el carril derecho.

![Datos de credencial de un recurso aprobado](./images/review-and-approve1.png){width="60%"}

Los detalles de credenciales por variante se muestran cuando los revisores inspeccionan los recursos. Las experiencias aprobadas se vuelven a firmar cuando los usuarios hacen clic en **[!UICONTROL Guardar en contenido]**.

![Datos de credencial de un recurso aprobado](./images/review-and-approve2.png)

### Activación y exportación

Durante la activación, el estado de las credenciales se muestra en el selector de experiencias.

![Datos de credencial de un recurso activado](./images/activate-export1.png){width="60%"}

Los archivos exportados tendrán credenciales compatibles con C2PA incrustadas.

La integridad de las credenciales se mantiene en todos los formatos admitidos (JPEG, PNG, MP4).

![Datos de credencial de un recurso exportado](./images/activate-export2.png)

