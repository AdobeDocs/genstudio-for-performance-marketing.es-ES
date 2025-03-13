---
title: Implemente su aplicación de App Builder
description: Implemente su aplicación de App Builder o complemento para GenStudio for Performance Marketing.
source-git-commit: acc54215d980f1f7392401cca9d90ed0ce41b2ec
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---


# Implemente la aplicación

La ejecución de la aplicación proporciona una instantánea preliminar del comportamiento del complemento antes de implementarlo. Esta información puede facilitar la depuración. Puede forzar la compilación y la implementación de una aplicación implementada sin volver a enviarla para su aprobación.


**Para ejecutar la aplicación**:

Ejecutar la aplicación en `https://localhost:9080`:

```bash
aio app run
```

**Para implementar la aplicación**:

1. Vaya al espacio de trabajo de implementación. Por ejemplo, para desplazarse al espacio de trabajo de producción:

   ```bash
   aio app use -w Production
   ```

1. Implemente la aplicación:

   ```bash
   aio app deploy
   ```

**Para forzar la reimplementación**:

>[!NOTE]
>
>Forzar la generación y la implementación sobrescribe la implementación existente. Pruebe exhaustivamente la aplicación primero en un entorno de prueba.

```bash
aio app build --force-build
```

```bash
aio app deploy --force-deploy
```

**Para generar e implementar al mismo tiempo**:

```bash
aio app deploy --force-build --force-deploy
```

**Para ver la aplicación**:

Después de la implementación, puede ver la aplicación en GenStudio for Performance Marketing agregando un parámetro `query` a la dirección URL de GenStudio for Performance Marketing:

`https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create`

Si está satisfecho con el complemento, está listo para distribuirlo sin el parámetro `query`.

Ahora puedes [distribuir tu aplicación](distribute-app.md).
