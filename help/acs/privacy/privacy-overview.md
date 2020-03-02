---
title: Privacy Requests with the Adobe Campaign Standard (ACS) - Overview
description: The tutorial explains how the create Privacy requests via the Adobe Campaign Standard (ACS) interface.
feature: GDPR, CCAP
topic: Privacy
kt: 1480
doc-type: feature video
activity: use
team: TM
---

# Privacy Requests with the Adobe Campaign Standard User Interface

Adobe Campaign offers Data Controllers three methods for performing Privacy access and delete requests of PII data in compliance with privacy acts such as GDPR (General Data Protection Regulation) and CCPA (California Consumer Privacy Act):

* **Via the Privacy Core Service integration:** Privacy requests pushed from the Privacy Core Service to all Experience Cloud solutions are automatically handled by Campaign via a dedicated workflow. Refer to the [Adobe Experience Platform Privacy Service](https://adobe.io/apis/cloudplatform/gdpr.html) to learn how to create Privacy requests from the Privacy Core Service
  
* **Via the API:** Adobe Campaign provides an API that allows the automatic process of Privacy requests using REST
  
* **Via the Adobe Campaign interface:** for each Privacy request, the Data Controller creates a new privacy request in Adobe Campaign

>[!NOTE]
>
> **CHANGES WITH ACS 19.4:**
> 
> The [Privacy Core Service integration](https://adobe.io/apis/cloudplatform/gdpr.html) is the method you should use for all access and delete requests. Starting 19.4, the >use of the Campaign API and interface for access and delete requests is deprecated. For more on Campaign Standard deprecated and removed features, refer to [this page](https://helpx.adobe.com/campaign/kb/acs-deprecated-and-removed-features.html).
>
>**Opt-out for the Sale of Personal Information (CCPA)**
>
>Starting with 19.4, a CCPA Opt-Out field is provided out-of-the-box in the Campaign interface and API. For 19.3, to leverage this information, you need to create this >field in Adobe Campaign Standard. Please see the [detailed documentation](https://helpx.adobe.com/campaign/kb/acs-privacy.html#ccpa) for more information.
>
> You can check your version by clicking on the ? icon in the top right of the interface and selecting About.

## Video Tutorials

### Prerequisites for Privacy Requests

1. [Create a Namespace](/help/acs/privacy/namespaces-for-privacy-requests.md)
2. [Modify Custom Resources](/help/acs/privacy/custom-resources-for-privacy-requests.md)

### Create,track and execute Privacy requests through the Adobe Campaign user interface

* [Create and track privacy requests through the Adobe Campaign user interface](/help/acs/privacy/create-and-track-privacy-requests.md)
* [Execute privacy requests](/help/acs/privacy/execute-privacy-requests.md)

## Additional Resources

* [General Privacy guidelines for Campaign](https://helpx.adobe.com/campaign/kb/campaign-privacy-overview.html)
* [CCPA for ACS](https://helpx.adobe.com/campaign/kb/acs-privacy.html#ccpa)
* [Adobe Experience Platform Privacy Service](https://adobe.io/apis/cloudplatform/gdpr.html)
* [Adobe Campaign Standard Rest API Documentation](https://final-docs.campaign.adobe.com/doc/standard/en/api/ACS_API.html#privacy-management)
