---
title: Administración de datos
description: Obtenga información acerca de la ingesta y el almacenamiento de datos para  [!DNL Insights] en GenStudio for Performance Marketing.
feature: Reporting and Insights
level: Experienced
role: Admin, Data Architect
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
source-git-commit: 44fedfdc3902b4f993d656ae6360a32e27a62520
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# Administración de datos

GenStudio for Performance Marketing usa Adobe Experience Platform (AEP) para la ingesta de datos y el almacenamiento de las métricas y los metadatos que alimentan [!DNL Insights]. AEP usa _esquemas_ para definir las estructuras de datos y _conjuntos de datos_ para almacenar y administrar las colecciones de datos.

## Conexiones de datos

GenStudio for Performance Marketing utiliza Customer Journey Analytics (CJA) para agregar varias fuentes de datos creando una conexión con uno o varios conjuntos de datos de AEP. CJA usa estas conexiones de datos para crear vistas de datos y analizar métricas con [!DNL Insights].

>[!BEGINSHADEBOX]

**Información importante acerca de conexiones de datos**

Si usted es administrador del sistema de [Adobe](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager), es posible que tenga derechos que permitan el acceso a la administración de la zona protegida de AEP y a los componentes del lago de datos que admiten GenStudio for Performance Marketing.

>[!WARNING]
>
>Al restablecer la zona protegida de producción en AEP, se eliminarán todas las conexiones de datos y [!DNL Insights] dejará de funcionar.

Tenga cuidado y no elimine las siguientes conexiones de datos necesarias para que GenStudio for Performance Marketing funcione de forma fiable:

- Conjuntos de datos de AEP con el prefijo `GS Insights`
- Esquemas, clases y grupos de campos de AEP con el prefijo `GS Insights`
- Grupo de campos personalizados `timestamp for metadata`
- Conexiones de AEP: flujos de datos con el prefijo `GS Insights`
- AEP Connections: cuenta de GS Insights

Consulte [Eliminar implicaciones](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion) en la guía de _Customer Journey Analytics_ antes de eliminar cualquier componente de datos en AEP.

>[!ENDSHADEBOX]

## Política de retención de datos

GenStudio for Performance Marketing retiene los datos de canal durante 13 meses. Esta política de retención incluye los 6 meses de datos introducidos durante la conexión inicial, lo que garantiza un análisis y unos informes de datos históricos completos.

Ver [Conectar cuenta de medios pagados](/help/user-guide/connectors/connect-channel.md).
