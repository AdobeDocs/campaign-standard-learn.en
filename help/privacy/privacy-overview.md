---
title: Privacy requests with the Adobe Campaign Standard (ACS) - Overview
description: The tutorial explains how the create privacy requests via the Adobe Campaign Standard interface.
feature: Privacy Tools
kt: 1480
doc-type: feature video
activity: use
team: TM
exl-id: fb766403-694c-4a7b-b3d1-4a418df85891
---
# Privacy requests with the Adobe Campaign Standard User Interface

Adobe Campaign offers data controllers three methods for performing Privacy access and delete requests of PII data in compliance with privacy acts such as GDPR (General Data Protection Regulation) and CCPA (California Consumer Privacy Act):

* **Via the Privacy Core Service integration:** Privacy requests pushed from [!UICONTROL Privacy Service] to all Experience Cloud solutions are automatically handled by Campaign via a dedicated workflow. To learn how to create privacy requests from the Privacy Core Service refer to the [Adobe Experience Platform Privacy Service](https://www.adobe.io/apis/experienceplatform/gdpr.html) 
  
* **Via the API:** Adobe Campaign provides an API that allows the automatic process of privacy requests using REST
  
* **Via the Adobe Campaign interface:** for each privacy request, the data controller creates a privacy request in Adobe Campaign

>[!NOTE]
>
> **CHANGES WITH ACS 19.4:**
> 
> The [Privacy Service integration](https://www.adobe.io/apis/experienceplatform/gdpr.html) is the method you should use for all access and delete requests. Starting 19.4, the use of the Campaign API and interface for access and delete requests is deprecated. For more on Campaign Standard deprecated and removed features, refer to [this page](https://experienceleague.adobe.com/docs/campaign-standard/using/release-notes/deprecated-features.html?lang=en).
>
>**Opt-out for the Sale of Personal Information (CCPA)**
>
> A CCPA Opt-Out field is provided out-of-the-box in the Campaign interface and API.
>
> You can check your version, click the **?** icon in the top right of the interface and selecting About.

## Video Tutorials

### Prerequisites for Privacy Requests

1. [Create a Namespace](/help/privacy/namespaces-for-privacy-requests.md)
1. [Modify custom resources](/help/privacy/custom-resources-for-privacy-requests.md)

### Create, track, and execute Privacy requests through the Adobe Campaign user interface

* [Create and track privacy requests through the Adobe Campaign user interface](/help/privacy/create-and-track-privacy-requests.md)
* [Execute privacy requests](/help/privacy/execute-privacy-requests.md)

## Additional resources

* [General Privacy Guidelines for Campaign](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/privacy/privacy-management.html?lang=en#getting-started)
* [CCPA for ACS](https://experienceleague.adobe.com/docs/campaign-standard/using/getting-started/privacy/privacy-requests.html?lang=en#privacy-requests)
* [Adobe Experience Platform Privacy Service](https://www.adobe.io/apis/experienceplatform/gdpr.html)
* [Adobe Campaign Standard REST API Documentation](https://final-docs.campaign.adobe.com/doc/standard/en/api/ACS_API.html#privacy-management)
