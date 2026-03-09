---
title: Administración de datos
description: Obtenga información acerca de la ingesta y el almacenamiento de datos para  [!DNL Insights] en GenStudio for Performance Marketing.
feature: Reporting and Insights
level: Experienced
role: Admin, Developer
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
TQID: https://experienceleague.adobe.com/HM2e0Yq2uwTpKtK-z8gHs0hDFrsJS6koQBqoNoKJK0Y
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: e0aa398c-6185-4e77-8cf7-2561c578c181
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: d3cdead0-685a-4489-9250-4bb709942f66
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 249
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
