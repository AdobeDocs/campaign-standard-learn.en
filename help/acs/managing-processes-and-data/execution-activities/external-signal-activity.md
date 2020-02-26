---
title: External Signal Activity - Call a workflow with parameters
seo-title: External Signal Activity - Call a workflow with parameters
description: The External Signal Activity is used to organize and orchestrate different processes that are part of the same customer journey into different workflows. It allows to start one workflow from another, enabling to support more complex customer journeys, while being able to better monitor and react in case of issue.
seo-description: The External Signal Activity is used to organize and orchestrate different processes that are part of the same customer journey into different workflows. It allows to start one workflow from another, enabling to support more complex customer journeys, while being able to better monitor and react in case of issue.
uuid: 4f640ae6-a532-4feb-80dd-fceee98e0b38
discoiquuid: 0e710e00-198b-42fe-9a55-2a8d86cca127
feature: External Signal Activity
topics: Execution  
kt: KT-2750 
doc-type: feature video
activity: use
team: TM
---

# External Signal Activity - Call a workflow with parameter

The External Signal Activity is used to organize and orchestrate different processes that are part of the same customer journey into different workflows. It allows to start one workflow from another, enabling to support more complex customer journeys, while being able to better monitor and react in case of issue.

In ACS 19.2 the External Signal Activity can not only call a workflow, but in addition pass parameters to the workflow (an audience name to target, a file name to import, a part of message content, etc.) to the workflow from another workflow or a REST API call to integrate with your external systems.

This also includes a new **Test** Activity where you can run tests on this functionality.

The video below explains the configuration steps required to:

1. **Receive external parameters** from an external system, like a content management system (CRM):
   * Declare the parameters in the External Signal Activity
   * Configure the API call to define the parameters and trigger the workflow External Signal Activity. For more information on how to configure an API call please see [Triggering a Signal Activity](https://docs.campaign.adobe.com/doc/standard/en/api/ACS_API.html#triggering-a-signal-activity).
  
2. **Customize a workflow with external parameters** (eventsvariables):
Once the workflow triggered, the parameters are ingested into the workflow's events variables and can be used within the workflow. See the [documentation](https://helpx.adobe.com/campaign/standard/automating/using/calling-a-workflow-with-external-parameters.html) for all activities that can be customized with event variables:
   * Configure the Test Activity (new in 19.2)
   * Configure Read Audience and Email Delivery Activity
3. **Configure an End Activity** to call a workflow with external parameters

>[!VIDEO](https://video.tv.adobe.com/v/27249/?quality=12)

## Additional Resources

* [External Signal (documentation)](https://docs.adobe.com/content/help/en/campaign-standard/using/managing-processes-and-data/data-management-activities/external-api.html)
