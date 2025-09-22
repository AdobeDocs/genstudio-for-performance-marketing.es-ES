---
title: Implemente su aplicación de App Builder
description: Implemente su aplicación de App Builder o complemento para GenStudio for Performance Marketing.
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
source-git-commit: 7fdd3f54a0a031bfe26b48983de9cd24baad2f62
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# Implemente la aplicación

La ejecución de la aplicación ofrece una instantánea preliminar del comportamiento del complemento antes de implementarlo. Esta información puede facilitar la depuración.

**Para ejecutar la aplicación**:

Ejecutar la aplicación en `https://localhost:9080`:

```bash
aio app run
```

**Para implementar la aplicación**:

1. Vaya al espacio de trabajo de implementación:

   ```bash
   aio app use -w [deployment_workspace]
   ```

2. Implemente la aplicación:

   ```bash
   aio app deploy
   ```

**Para forzar la reimplementación**:

Puede forzar una compilación e implementación de su aplicación sin volver a enviarla para su aprobación.

>[!NOTE]
>
>Forzar una compilación e implementación sobrescribe la implementación existente. **Primero pruebe exhaustivamente su aplicación** en un entorno de prueba.

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

```txt
https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create
```

Si está satisfecho con el complemento, está listo para distribuirlo sin el parámetro `query`.

Ahora puedes [distribuir tu aplicación](distribute-app.md).
