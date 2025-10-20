---
title: GenStudio Experience Selector MFE
description: Comprenda e implemente el Micro FrontEnd del selector de experiencias para sus aplicaciones y complementos de GenStudio.
feature: Extensibility, Extensions, Experiences
source-git-commit: 2d6453274d1bfeb35df2821e7e31eec1ca87b013
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 6%

---

# GenStudio Experience Selector MFE

El Selector de experiencias es un Micro Frontend (MFE) que proporciona un componente `ExperienceSelectorDialog` para seleccionar experiencias de GenStudio. Utilice el componente en su aplicación importando la función `renderExperienceSelectorWithSUSI` del paquete independiente de JavaScript, que carga automáticamente el último Micro Frontend implementado y presenta una interfaz de componente natural.

El MFE Selector de experiencias de GenStudio permite a los usuarios:

- Busque y seleccione experiencias de GenStudio
- Filtrar experiencias según varios criterios
- Admite modos de selección única y múltiple
- Administrar la autenticación mediante la integración de SUSI (inicio de sesión de registro)
- Proporcionar una IU coherente en los distintos marcos de trabajo

## Opciones de integración

El MFE puede integrarse utilizando dos métodos diferentes:

### ESM (Módulos ES): recomendado

```javascript
import { renderExperienceSelectorWithSUSI } from 'https://experience.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/esm/standalone.js';
```

### UMD (Definición de módulo universal)

```html
<script src="https://experience.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/umd/standalone.js"></script>
```

## Propiedades de configuración

La función `renderExperienceSelectorWithSUSI` acepta un objeto de configuración con las siguientes propiedades:

| Propiedad | Tipo | Requerido | Descripción |
|----------|------|----------|-------------|
| `apiKey` | cadena | Sí | Clave de API para servicios de GenStudio |
| `imsOrg` | cadena | Sí | ID de organización IMS |
| `env` | cadena | Sí | Entorno (`stage`, `prod`) |
| `susiConfig` | objeto | Sí | [Configuración de autenticación SUSI](#susi-configuration) |
| `onSelectionConfirmed` | función | Sí | Llamada de retorno cuando se confirma la selección |
| `onDismiss` | función | Sí | Llamada de retorno cuando se cierra el diálogo |
| `locale` | cadena | No | Configuración regional del idioma (por ejemplo, `en-US`) |
| `isOpen` | booleano | No | Estado del cuadro de diálogo inicial |
| `selectionType` | cadena | No | El modo de selección (`single` o `multiple`) |
| `customFilters` | matriz | No | Criterios de filtro personalizados |
| `dialogTitle` | cadena | No | Título del cuadro de diálogo personalizado |

### Configuración de SUSI

El objeto `susiConfig` puede incluir:

```javascript
{
  clientId: 'genstudio',
  environment: 'stg1', // or 'prod'
  scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
  locale: 'en_US',
  modalSettings: {
    width: 500,
    height: 700
  }
}
```

## QuickStart

1. **Elija su módulo** entre los ejemplos disponibles a continuación
1. **Vaya al directorio de ejemplo**
1. **Instalar dependencias** (para ejemplos de React/Vue)
1. **Actualice la configuración** con sus claves API y la organización IMS:

   ```javascript
   const experienceSelectorProps = {
     locale: 'en-US',
     apiKey: 'exc_app',           
     imsOrg: 'your-ims-org@AdobeOrg',  // Replace with your IMS Org
     env: 'stage', // or 'prod'
     susiConfig: {
        clientId: 'genstudio',
        environment: 'stg1', // or 'prod'
        scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
        locale: 'en_US',
        modalSettings: {
          width: 500,
          height: 700,
        },
     },
     customFilters: ['genstudio-channel:email'],
     selectionType: 'single', // or 'multiple'
     dialogTitle: 'Select Email Templates'
   };
   ```

1. **Ejecutar el servidor de desarrollo**

### Implementaciones de ejemplo

Este repositorio incluye ejemplos de trabajo para diferentes marcos:

- [Una **aplicación React completa** que muestra la integración con el sistema de compilación de Vite](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/react-js).

- [Una aplicación **Vue 3** con integración de API de composición](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vue-js).

- [Dos **implementaciones de Vanilla JavaScript**](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js):

   - [Esta versión de **ESM de vainilla** usa módulos ES6 y JavaScript moderno](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-esm).

   - [Esta versión de **UMD de vainilla** usa el paquete UMD cargado mediante la etiqueta de script](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-umd-global-var).

## Flujo de autenticación

El Selector de experiencia administra la autenticación automáticamente mediante SUSI:

1. Cuando se abre el cuadro de diálogo, comprueba la autenticación existente.
1. Si no se autentica, se abre un flujo de inicio de sesión SUSI.
1. Después de la autenticación correcta, se muestra el selector de experiencia.
1. Los usuarios pueden examinar y seleccionar experiencias.
1. Las experiencias seleccionadas se devuelven mediante la llamada de retorno `onSelectionConfirmed`.
