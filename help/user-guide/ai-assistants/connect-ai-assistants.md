---
title: Conectar un asistente de IA
description: Aprenda a conectar un asistente de IA compatible a [!DNL GenStudio for Performance Marketing] y a verificar el acceso a las herramientas disponibles.
role: User
source-git-commit: 3d22af77d3893233e497a22f7b00c1faf0070cff
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%
---

# Conectar un asistente de IA

Conecte un asistente de IA admitido a [!DNL GenStudio for Performance Marketing] antes de consultar los datos de rendimiento, montar borradores o publicar anuncios aprobados. Las opciones de conexión varían según el asistente y la organización de IA.

## Requisitos previos

Antes de conectarse, confirme lo siguiente:

- Una cuenta activa de Adobe con acceso a [!DNL GenStudio for Performance Marketing].
- Un plan compatible que permite conexiones MCP remotas cuando utiliza Claude, ChatGPT o Microsoft Copilot. Consulte la documentación del asistente de IA para obtener instrucciones específicas sobre la configuración manual de conexiones MCP.

## Conectar Adobe CX Enterprise Coworker

[!DNL GenStudio for Performance Marketing] herramientas se administran como una conexión nativa en Adobe CX Enterprise Coworker. Su organización controla la disponibilidad, por lo que no introduce la dirección URL directa del servidor MCP.

Iniciar una nueva conversación y [comprobar la conexión](#verify-the-connection). Si no aparecen las herramientas, póngase en contacto con el administrador de su organización o con un representante de Adobe.

## Conectar Claude

Claude requiere un plan Pro, Max, Team o Enterprise. El mismo conector remoto funciona en Claude en la web y en la aplicación de escritorio.

1. En Claude, seleccione **[!UICONTROL Personalizar]** en la barra lateral izquierda.
1. Seleccione **[!UICONTROL Conectores]** y luego seleccione el icono Agregar.
1. Seleccione **[!UICONTROL Agregar conector personalizado]**.
1. Escriba `https://genstudio-services.adobe.io/mcp` como URL del servidor MCP.
1. Inicie sesión con su Adobe ID.
1. Seleccione la organización de IMS que tiene acceso a [!DNL GenStudio for Performance Marketing].

>[!NOTE]
>
>En un plan de equipo o de empresa, es posible que el propietario de una organización tenga que agregar primero el conector. Si el conector ya está disponible, selecciona **[!UICONTROL Conectar]** en su lugar.

## Conectar ChatGPT

ChatGPT requiere una cuenta Plus, Pro, Business, Enterprise o Education. Las conexiones MCP personalizadas están disponibles en la web a través del modo de desarrollador.

1. Inicie sesión en [ChatGPT](https://chatgpt.com) en un explorador web.
1. Abra **[!UICONTROL Configuración]** y habilite **[!UICONTROL Modo de desarrollador]**.
1. En **[!UICONTROL Configuración]**, abra el área de aplicaciones o conectores.
1. Agregue una conexión MCP personalizada denominada `GenStudio`.
1. Escriba `https://genstudio-services.adobe.io/mcp` como URL del servidor MCP.
1. Mantenga **[!UICONTROL OAuth]** como método de autenticación.
1. Inicie sesión con su Adobe ID.
1. Seleccione la organización de IMS que tiene acceso a [!DNL GenStudio for Performance Marketing].

>[!NOTE]
>
>ChatGPT puede cambiar la ubicación del desarrollador y la configuración del conector. Si estas etiquetas difieren en su cuenta, siga las instrucciones actuales de OpenAI para agregar un conector MCP remoto.

## Códice de Connect

El Codex requiere la interfaz de línea de comandos del Codex y una cuenta autenticada del Codex.

1. Abra `~/.codex/config.toml` para todos los proyectos o `.codex/config.toml` para un proyecto.
1. Añada esta configuración:

   ```toml
   [mcp_servers.genstudio]
   url = "https://genstudio-services.adobe.io/mcp"
   auth = "oauth"
   ```

1. Ejecutar `codex mcp login genstudio`.
1. Inicie sesión con su Adobe ID en la ventana del explorador que se abre.
1. Seleccione la organización de IMS que tiene acceso a [!DNL GenStudio for Performance Marketing].

## Conectar escritor

Writer requiere acceso a AI Studio.

1. En Writer, abra **[!UICONTROL AI Studio]**.
1. Seleccione **[!UICONTROL Conectores y herramientas]**.
1. Seleccione **[!UICONTROL Crear conector personalizado]**.
1. Seleccione **[!UICONTROL Servidor MCP]** como tipo de conector.
1. Introduzca un nombre y una descripción para el conector.
1. Escriba `https://genstudio-services.adobe.io/mcp` como URL del servidor MCP.
1. Configure el acceso de equipo del conector.
1. Seleccione **[!UICONTROL OAuth 2.0 (nivel de usuario)]** como método de autenticación.
1. Inicie sesión con su Adobe ID.
1. Seleccione **[!UICONTROL Guardar]**.

[!DNL GenStudio for Performance Marketing] herramientas aparecen en la biblioteca de herramientas de AI Studio. Cada usuario de Writer inicia sesión con un Adobe ID individual.

## Conectar Microsoft Copilot

Microsoft controla el flujo de configuración para las conexiones MCP personalizadas en Copilot. Siga la [documentación actual de Microsoft Copilot](https://learn.microsoft.com/en-us/copilot/) para agregar un servidor MCP remoto y luego use `https://genstudio-services.adobe.io/mcp` como URL del servidor.

Cuando se le solicite, inicie sesión con su Adobe ID y seleccione la organización de IMS que tiene acceso a [!DNL GenStudio for Performance Marketing].

## Comprobar la conexión

Después de la configuración, confirme que las herramientas están disponibles.

1. Inicie una nueva conversación en su asistente de IA.
1. Pregunte al asistente a qué herramientas de [!DNL GenStudio for Performance Marketing] puede acceder.
1. Confirme que la respuesta enumera las herramientas en Perspectivas, Crear y Activar.
1. Solicite un resumen de rendimiento para un canal de medios de pago conectado.

El asistente devuelve los datos de rendimiento disponibles o explica por qué no coinciden los datos con la solicitud.

>[!TIP]
>
>Si la autenticación falla, vuelva a conectarse y confirme que ha seleccionado la organización IMS correcta. Si no aparece ninguna herramienta, confirme que su cuenta tiene acceso a [!DNL GenStudio for Performance Marketing].

## Funciones relacionadas

- [Información general sobre asistentes de IA](overview.md)
- [Uso de asistentes de IA](use-ai-assistants.md)
- [Referencia de herramientas del asistente de IA](tools-reference.md)
