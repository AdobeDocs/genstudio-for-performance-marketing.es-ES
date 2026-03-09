---
title: Adobe GenStudio for Performance Marketing Campaigns
description: Aprenda a crear y administrar campañas de marketing digital que aprovechen los recursos y las experiencias de IA generativa.
feature: Campaign Planning, Campaign Brief
badgeBeta: label="Beta" tooltip="Esta función se encuentra actualmente en Beta, por lo que algunas funciones pueden estar limitadas o sujetas a cambios."
exl-id: b7c4194f-fa61-4739-acd6-7acbdd98e9b2
TQID: https://experienceleague.adobe.com/fcmU2HDzq75iNR7LlKqMcANCa67FpA0fFelMhkQtOJk
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
  - id: b286a442-6f0d-405a-adea-abb4a98e2d7b
  - id: bf1f49e6-dcda-4b68-a4d5-aeecf05031a6
  - id: dd48f9df-f2e2-49fe-a918-332a8e240ffe
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: beb7a3c1-66ab-4786-b879-7621375b3c40
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 866
ht-degree: 0%

---

# Creación de una campaña

Una campaña de GenStudio for Performance Marketing define los rasgos clave de la campaña digital y evoluciona a medida que se implementan y evalúan las fases. GenStudio for Performance Marketing admite el proceso dinámico de inicio de una campaña, seguimiento del rendimiento de componentes de campaña individuales y reorientación de las experiencias de publicidad en función de las métricas de rendimiento.

Los elementos clave de la campaña se almacenan en un objeto de campaña, lo que crea un contexto compartido para todos los recursos y experiencias etiquetados con el mismo nombre de campaña único. Esta etiqueta identifica la campaña en GenStudio for Performance Marketing.

Los administradores del sistema de GenStudio y los editores de GenStudio pueden crear campañas.

## Definición de detalles de campaña

{{$include /help/_includes/campaign-details.md}}

**Para ingresar los detalles de la campaña**:

1. Desde [!DNL Campaigns], haga clic en **[!UICONTROL Agregar campaña]**. Se abre la vista _Crear una campaña_.

   Los detalles abarcan campos opcionales y obligatorios que definen la campaña. Estos detalles se guardan en [!DNL Campaigns] como atributos de metadatos de la campaña.

1. Haga doble clic en el encabezado _Nueva campaña_ e introduzca un nombre único e informativo.

   Este nombre se convierte en _etiqueta de campaña_ en GenStudio for Performance Marketing, lo que le permite asociar recursos o experiencias con la campaña durante la carga y la creación.

1. Escriba valores en _Detalles_ campos que describan su campaña. Consulte la tabla _Detalles de campaña_ para ver las definiciones de estas características de campaña.

## Asignar canales y regiones

La configuración de canal y región determina dónde se implementa la campaña y sus canales de distribución.

GenStudio for Performance Marketing usa plantillas predefinidas denominadas _registros_ para representar componentes clave de la campaña, como canales, regiones, personalidades y productos. Al crear una campaña, se asocia con los registros relevantes para cada uno de estos componentes.

* **Configuración de canal**: define los canales de distribución pública para su campaña, incluidas las cuentas de medios de pago, los servicios de marketing por correo electrónico y las redes de anuncios en pantalla. Los datos sobre el rendimiento de las campañas, los recursos y las experiencias de estos canales se incluyen en [[!DNL Insights]](/help/user-guide/insights/overview.md) para su análisis específico del canal.

* **Configuración de región**: especifica las áreas geográficas en las que implementa la campaña. Al conectar con fuentes de datos regionales, GenStudio for Performance Marketing puede adaptar el contenido y la estrategia a las preferencias de audiencia locales. Esto permite una segmentación y un análisis del rendimiento más precisos en función de las métricas regionales.

**Para seleccionar canales de distribución para su campaña**:

1. Haga clic en el signo + (**[!UICONTROL Conectar registros +]**) junto a **[!UICONTROL Canales]**.

   Se abre la ventana emergente _Seleccionar canales_.

1. Seleccione los canales en los que se implementa la campaña. Los valores válidos incluyen `Email`, `Paid media`, `Web` y `Display ads`.

   De manera opcional, elige **[!UICONTROL Ver todo]** para abrir una vista de todos los canales admitidos.

**Para asignar regiones a tu campaña**:

1. Haga clic en el signo + (**[!UICONTROL Conectar registros +]**) junto a **[!UICONTROL Regiones]**.

   Se abre la ventana emergente _Seleccionar regiones_. Puede buscar una región compatible específica.

1. Seleccione las regiones o más regiones de destino para la campaña. Las regiones válidas incluyen `AMER`, `LATAM`, `EMEA`, `APAC` y `Japan`.

   De manera opcional, elija **[!UICONTROL Ver todo]** para abrir una vista de todas las regiones compatibles.

## Asignar perfiles y productos

[Los personajes](/help/user-guide/guidelines/personas.md) y [productos](/help/user-guide/guidelines/products.md) se guardan como registros. Un registro personal define las características de un segmento de cliente específico: la audiencia de destino para el contenido generado. Puede incluir detalles demográficos y un historial de interacciones de clientes.

Los registros de productos definen las especificaciones y atributos clave del producto en el contexto de las directrices de marca. Los atributos pueden incluir funciones, imágenes asociadas y la posición del producto dentro de la marca.

Las opciones de los menús desplegables _Personas_ y _Productos_ se definen en el nivel de organización. Al crear una campaña, puede seleccionar entre estos registros predefinidos para garantizar una representación del producto coherente y admitir un direccionamiento, un mensaje y un seguimiento del rendimiento precisos.

**Para asignar personalidades a tu campaña**:

1. Haga clic en el signo + (**[!UICONTROL Conectar registros +]**) junto a **[!UICONTROL Personas]**.

   Se abre la ventana emergente _Seleccionar personalidades_. Puede buscar una persona compatible específica.

1. Seleccione los perfiles a los que se dirige su campaña. Su organización ha definido los perfiles válidos durante la [creación de directrices](/help/user-guide/guidelines/personas.md).

   De manera opcional, elige **[!UICONTROL Ver todo]** para abrir una vista de todas las personalidades disponibles.

**Para asignar productos a tu campaña**:

1. Haga clic en el signo + (**[!UICONTROL Conectar registros +]**) junto a **[!UICONTROL Productos]**.

   Se abre la ventana emergente _Seleccionar productos_. Puede buscar un producto compatible específico.

1. Seleccione uno o varios productos. Su organización define los productos durante la [creación de directrices](/help/user-guide/guidelines/products.md).

   De manera opcional, elige **[!UICONTROL Ver todo]** para abrir una vista de todos los productos disponibles.

## Creación completa de la campaña

Haga clic en **[!UICONTROL Crear]** para guardar los valores introducidos y crear la campaña.

El nuevo nombre de campaña ya está disponible como etiqueta de campaña en [!DNL Content] y [!DNL Create]. Puede agregar recursos y experiencias aprobados a su campaña a través de [!DNL Content], o asignar un recurso y una experiencia a una campaña durante la creación de contenido.

## Añadir contenido a la campaña

GenStudio for Performance Marketing vincula el contenido a las campañas mediante etiquetas de campaña almacenadas en los metadatos de [!DNL Content]. Un solo fragmento de contenido se puede asociar con varias campañas.

Las etiquetas de campaña identifican la campaña y sus atributos. La asignación de una etiqueta a un recurso o experiencia lo conecta con la campaña correspondiente.

**Para agregar recursos y experiencias de[!DNL Content]**:

1. En las galerías [!DNL Content] _Experiencias_ o _Assets_, elija la experiencia o el recurso aprobado.

1. En la vista _Detalles_, seleccione el nombre de la campaña en el menú desplegable _Campañas_.

**Para agregar recursos y experiencias durante la creación de contenido**:

Durante la creación de contenido, puede publicar el recurso o la experiencia recién creados en [!DNL Content].

1. En la ventana emergente _Confirmar detalles del contenido aprobado_, selecciona una campaña del menú desplegable _Campañas_.

1. Haga clic en **[!UICONTROL Publicar]**.

Esta campaña ya está disponible en el panel _Campañas_.
