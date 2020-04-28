---
title: Understanding the Adobe Experience Platform Data Connector
description: Adobe Experience Platform Data Connector helps existing customers to make their data available on Adobe Experience Platform by mapping XTK data (data ingested in Campaign) to Experience Data Model (XDM) data on Adobe Experience Platform.
feature: Adobe Experience Platform Data Connector
topics: ACoP
kt: 2826
doc-type: feature video
activity: understand
team: TM
---

# Understanding the Adobe Experience Platform [!UICONTROL Data Connector]

>[!NOTE]
>
>This capability is currently in beta, and subject to frequent updates and modifications without notice.
>Please reach out to [!UICONTROL Adobe Customer Support] if you plan to implement this capability.

## Overview

Adobe Experience Platform [!UICONTROL Data Connector] helps existing customers to make their data available on Adobe Experience Platform by mapping XTK data (data ingested in Adobe Campaign) to [!DNL Experience Data Model] (XDM) data on Adobe Experience Platform.

Note that the connector is uni-directional and sends the data from Adobe Campaign Standard to Adobe Experience Platform. The data is never sent from the Adobe Experience Platform to Adobe Campaign Standard.

Adobe Experience Platform [!UICONTROL Data Connector] is intended for data engineers who understand Adobe Campaign Standard [!UICONTROL custom resources] and have an understanding of how customer's overall data schema should be inside Adobe Experience Platform.

>[!VIDEO](https://video.tv.adobe.com/v/27304?quality=12)

*This video gives an overview over the Adobe Experience Platform [!UICONTROL Data Connector] (09:35 min)*

>[!NOTE]
>
>The out-of-the-box transfer of [!UICONTROL subscription events] is not supported. To transfer [!UICONTROL subscription events], you can create corresponding XDM and dataset on Adobe Experience Platform, then configure a custom data mapping for these data.
>Existing [!UICONTROL experience events] cannot be ingested into Adobe Experience Platform, but ongoing generated [!UICONTROL experience events] will be streamed to Adobe Experience Platform.

## Key steps to perform a data mapping

The following tutorials describe the key steps to perform a data mapping between Campaign Standard and Adobe Experience Platform:

1. [Mapping Custom Resources](/help/administrating/adobe-experience-platform-data-connector/mapping-custom-resources.md)
2. [Mapping Experience Events](/help/administrating/adobe-experience-platform-data-connector/mapping-experience-events.md)
3. [Mapping Seed Table Data](/help/administrating/adobe-experience-platform-data-connector/mapping-seed-table-data.md)
4. [Modifying the Data Mapping](/help/administrating/adobe-experience-platform-data-connector/modifying-data-mapping.md)
5. [Checking the status of a data ingestion jobs](/help/administrating/adobe-experience-platform-data-connector/checking-status-of-data-ingestion-jobs.md)

## Additional resources

* [About Adobe Experience Platform Data Connector](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-about-data-connector.html)
* [Experience Data Model overview](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-data-model-overview.html)
* [Mapping definition](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-mapping-definition.html)
* [Mapping activation](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-mapping-activation.html)
* [Triggering data ingestion through APIs](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-triggering-data-ingestion.html)
