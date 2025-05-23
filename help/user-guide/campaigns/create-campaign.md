---
title: Adobe GenStudio for Performance Marketing Campaigns
description: Aprenda a crear y administrar campañas de marketing digital que aprovechen los recursos y las experiencias de IA generativa.
feature: Campaign Planning, Campaign Brief
badgeBeta: label="Beta" tooltip="Esta función se encuentra actualmente en Beta, por lo que algunas funciones pueden estar limitadas o sujetas a cambios."
source-git-commit: edbeb7f0d08e2215a23f15cfeff77a5217cd264b
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 0%

---

# Creación de una campaña

Una campaña de GenStudio for Performance Marketing define los rasgos clave de la campaña digital y evoluciona a medida que se implementan y evalúan las fases. GenStudio for Performance Marketing admite el proceso dinámico de inicio de una campaña, seguimiento del rendimiento de componentes de campaña individuales y reorientación de las experiencias de publicidad en función de las métricas de rendimiento.

Los elementos clave de la campaña se almacenan en un objeto de campaña, lo que crea un contexto compartido para todos los recursos y experiencias etiquetados con el mismo nombre de campaña único. Esta etiqueta identifica la campaña en GenStudio for Performance Marketing.

Los administradores de sistemas de GenStudio y los editores de Genstudio pueden crear campañas.

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
