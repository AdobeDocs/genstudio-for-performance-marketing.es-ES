---
title: Creación de una aplicación de App Builder para ampliar GenStudio for Performance Marketing
description: Comience a crear una aplicación o un complemento.
feature: Extensibility
exl-id: 4e757dd4-a02d-472c-bc13-6f27dffa48f2
source-git-commit: 52e8e078bc013fe686b5cc2105089f7098cce575
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---

# Desarrollo de una aplicación de App Builder

Los desarrolladores que amplían las capacidades nativas de GenStudio for Performance Marketing usan [Adobe App Builder](https://developer.adobe.com/app-builder/) para crear, enviar e implementar sus aplicaciones ampliables o complementos.

>[!BEGINSHADEBOX]

**Requisitos previos**:

* Node.js (versión 20.x o superior)

* npm (empaquetado con Node.js)

* Interfaz de línea de comandos (CLI) de Adobe Developer. Para instalar: `npm install -g @adobe/aio-cli`

>[!ENDSHADEBOX]

## Estructura de aplicación

Los complementos de GenStudio for Performance Marketing son aplicaciones de App Builder y contienen los mismos componentes básicos que otras aplicaciones de App Builder.

### Archivos de compilación y configuración

Los componentes clave de las aplicaciones de App Builder incluyen estos archivos de compilación y configuración. Esta lista no incluye todos los archivos de compilación y configuración.

* `README.md`: incluye información general sobre la aplicación.

* Archivos de aplicación TS:

   * `package.json`
   * `package-lock.json`
   * `eslint`
   * `tsconfig`
   * `jest test up`

* Archivos de configuración de App Builder:

   * `app.config.yaml`
   * `ext.config.yaml`: archivo de configuración para el complemento
   * `app.config.yaml`: archivo de configuración para el complemento (incluye la definición de su aplicación como complemento de GenStudio for Performance Marketing)
   * `.aio`
   * `.env`: no comprometa el archivo `.env` con el control de código fuente

### código Source

```
- src/
    - genstudiopem/
        - web-src/
            - src/
                - components/
                - utils/
                - Constants.ts
                - index.tsx
                - index.css
                - utils.ts
        - index.html
```

### Componentes de código Source

* `ExtensionRegistration.tsx`: define las API necesarias que la aplicación host (GenStudio for Performance Marketing) necesita para cargar y mostrar el complemento.

* `App.tsx`: componente de la aplicación principal que define el enrutamiento a otros componentes.

* `AdditionalContextDialog.tsx`: componente de diálogo para mostrar complementos de contexto adicionales.

* `RightPanel.tsx`: componente de diálogo para un complemento de validación.

* `Helper` componentes: incluye `ClaimsChecker`.

## Creación de una aplicación de App Builder a partir de una aplicación existente

Puede utilizar una aplicación de ejemplo para iniciar la creación de su complemento.

**Para crear una aplicación de App Builder a partir de una aplicación existente**:

1. Descargue una aplicación de ejemplo del repositorio [GenStudio UIX Examples](https://github.com/adobe/genstudio-uix-examples).

1. En el área de trabajo del proyecto App Builder en [Adobe Developer Console](https://developer.adobe.com/console/), seleccione **[!UICONTROL Descargar todo]** para descargar los detalles del proyecto.

1. Abra la aplicación de ejemplo localmente en el entorno de desarrollo integrado (IDE) que prefiera.

1. Autenticar con la interfaz de línea de comandos de Adobe Developer:

   ```bash
   aio login
   ```

1. Descargue el archivo JSON y, a continuación, cree su aplicación:

   ```bash
   aio app use '/path/to/your/downloaded/app-builder/project/details/config.json'
   ```

## Añadir código personalizado al complemento.

Usted define su código de complemento en `AdditionalContextDialog.tsx` y `RightPanel.tsx` archivos. Estos dos archivos definen el aspecto y el comportamiento de las ventanas emergentes cuando los usuarios acceden al complemento.

* `AdditionalContextDialog.tsx`: defina este componente si planea usar el complemento _Agregar contexto_. Los usuarios interactúan con este componente al hacer clic en _Complementos_ en el cajón de mensajes de [!DNL Create].

* `RightPanel.tsx`: defina este componente si planea usar el complemento _Panel derecho_ (validación de experiencia). Los usuarios interactúan con este componente al hacer clic en el complemento de validación en el panel derecho en un borrador de experiencia de [!DNL Create].

Ya está listo para [Implementar su aplicación](deploy-app.md)

## Prácticas recomendadas para el desarrollo de aplicaciones

El mantenimiento del entorno de desarrollo puede ayudarle a evitar errores de desarrollo e implementación de aplicaciones:

* Si utiliza una versión anterior de una aplicación de ejemplo, actualice las dependencias reinstalándolas:

  ```bash
  rm -rf node_modules package-lock.json && npm i
  ```

* Actualice GenStudio UIX SDK. Confirme que está usando la versión más reciente de [GenStudio UIX SDK](https://github.com/adobe/genstudio-uix-sdk). Consulte [Repositorio de ejemplo de UIX de GenStudio](https://github.com/adobe/genstudio-uix-examples) para obtener información sobre cómo usar los cambios más recientes de SDK.
