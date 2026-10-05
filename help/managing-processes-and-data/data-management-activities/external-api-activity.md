---
title: Configure and run a workflow with the External API activity
description: Learn you how to call an external REST API endpoint to pull personalization data from a third-party system into your campaign.
feature: Data Management Activity
jira: KT-2764
thumbnail: 28200.jpg
doc-type: feature video
activity: use
team: TM
exl-id: bce6fa2e-a684-43af-a41e-dfec54dd453a
role: User, Developer
level: Experienced
TQID: 'https://experienceleague.adobe.com/XTIqOfVTs-cE00YQM955S-7G1jwAU-W4pg1J8bNm-HE'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: f5407121-8933-4ac3-8e06-a9b692a4e88a
    internal-label: Campaign Standard
feature_v2:
  - id: a658c786-869b-4194-a780-2594d663adda
    internal-label: Data management
subfeature_v2:
  - id: 97f7b899-98c8-5133-9446-bfaf99a51b9f
    internal-label: Data Management Activity
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
    internal-label: Data management
---
# Configure and run a workflow with the [!UICONTROL External API activity]

The [!UICONTROL External API activity] is a [!UICONTROL Data Management activity]. It allows you to call an external REST API endpoint. The purpose of this activity is to get personalization data from a third-party system into your campaign.

Example use cases include:

* Getting the latest game-day lineup for a sports event to personalize content
* Getting the latest set of offers
* Connecting to a coupon generation system
* Checking the weather in local regions and using it to personalize content

This video demonstrates the use of the [!UICONTROL External API activity].

>[!VIDEO](https://video.tv.adobe.com/v/28200/?learn=on){transcript=true}

*[!UICONTROL External API activity] (06:48 min)*

>[!NOTE]
>
>The activity is meant for fetching campaign-wide data, not for retrieving specific information for each profile as that can result in large amounts of data being transferred. If the use case requires profile-specific information, the recommendation is to use the Transfer File activity.
