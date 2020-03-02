---
title: Configure and run a workflow with the External API activity
description: The External API activity brings data into the workflow from an external system via a REST API call. 
feature: External API Activity
topics: Data Management   
kt: 2764
doc-type: feature video
activity: use
team: TM
---

# Configure and run a workflow with the External API activity (beta)

The External API activity is a Data Management activity. It allows easy data ingress and egress with REST API systems for batch and blast workflows. 

The External API activity is meant for realtime fetching of campaign wide data (latest set of offers, latest scores etc.) not for retrieving specific information for each profile.  It enables a connection to Adobe I/O Runtime and similar systems (Azure Functions, AWS Lambda) from the workflow

Example use cases:

* Getting the latest game-day lineup for a sports event to personalize content
* Getting the latest set of offers
* Connecting to a coupon generation system
* Checking the weather in local regions and using it to personalize content (each zip code used could potentially retrieve its own local temperature
  
  >[!VIDEO](https://video.tv.adobe.com/v/28200/?quality=12)
  
  *External API Activity (min 04:12)*

>[!NOTE]
>
>This capability is currently in public beta. You need to accept the usage agreement before starting using the External API activity. Please note that since this public
>beta capability has not yet been commercially released by Adobe, it is not supported by Adobe Client Care, it may contain errors and may not function as well as other released features.
>

## Additional Resources

* [External API (Documentation)](https://docs.adobe.com/content/help/en/campaign-standard/using/managing-processes-and-data/data-management-activities/external-api.html)
  