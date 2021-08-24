---
title: Understand the Adobe Experience Platform Data Connector
description: Adobe Experience Platform Data Connector helps existing customers to make their data available on Adobe Experience Platform by mapping XTK data (data ingested in Campaign) to Experience Data Model (XDM) data on Adobe Experience Platform.
feature: People Core Service Integration
kt: 2826
thumbnail: 27304.jpg
doc-type: feature video
activity: understand
team: TM
exl-id: 686961f9-5374-4cc6-8b36-7ee0584ea720
---
# Understand the Adobe Experience Platform [!UICONTROL Data Connector]

>[!NOTE]
>
>This capability is in beta, and subject to frequent updates and modifications without notice.
>
>Please reach out to [!UICONTROL Adobe Customer Support] if you plan to implement this capability.

## Overview

Adobe Experience Platform [!UICONTROL Data Connector] helps existing customers to make their data available on Adobe Experience Platform by mapping XTK data (data ingested in Adobe Campaign) to [!DNL Experience Data Model] (XDM) data on Adobe Experience Platform.

The connector is uni-directional and sends the data from Adobe Campaign Standard to Adobe Experience Platform. The data is never sent from the Adobe Experience Platform to Adobe Campaign Standard.

Adobe Experience Platform [!UICONTROL Data Connector] is intended for data engineers who understand Adobe Campaign Standard [!UICONTROL custom resources] and have an understanding of how customer's overall data schema should be inside Adobe Experience Platform.

>[!VIDEO](https://video.tv.adobe.com/v/27304?quality=12)

*This video gives an overview over the Adobe Experience Platform [!UICONTROL Data Connector] (09:35 min)*

>[!NOTE]
>
>The out-of-the-box transfer of [!UICONTROL subscription events] is not supported. To transfer [!UICONTROL subscription events], you can create corresponding XDM and dataset on Adobe Experience Platform, then configure a custom data mapping for these data.
>
>Existing [!UICONTROL experience events] cannot be ingested into Adobe Experience Platform, but ongoing generated [!UICONTROL experience events] are streamed to Adobe Experience Platform.

## Key steps to perform a data mapping

The following tutorials describe the key steps to perform a data mapping between Campaign Standard and Adobe Experience Platform:

1. [Mapping Custom Resources](/help/administrating/adobe-experience-platform-data-connector/mapping-custom-resources.md)
2. [Mapping Experience Events](/help/administrating/adobe-experience-platform-data-connector/mapping-experience-events.md)
3. [Mapping Seed Table Data](/help/administrating/adobe-experience-platform-data-connector/mapping-seed-table-data.md)
4. [Modifying the Data Mapping](/help/administrating/adobe-experience-platform-data-connector/modifying-data-mapping.md)
5. [Check the status of a data ingestion job](/help/administrating/adobe-experience-platform-data-connector/checking-status-of-data-ingestion-jobs.md)

## Additional resources

* [About Adobe Experience Platform Data Connector](https://experienceleague.adobe.com/docs/campaign-standard/using/integrating-with-adobe-cloud/adobe-experience-platform/data-connector/aep-about-data-connector.html)
  