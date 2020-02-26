---
title: In-App Messaging Introduction
description: The Adobe Campaign Standard (ACS) In-App Messaging channel allows you to present the user with contextually relevant In-App messages in response to a customer's real-time behavior within the mobile application.
uuid: 50a13c41-88ad-43c4-8c42-d941bca2bf0a
discoiquuid: a3c10847-6163-4915-aae5-6200cd0474e5
feature: In-App
topics: Channels
kt: KT-1911
doc-type: feature video
activity: use
team: TM
---

# In-App Messaging Overview

The In-App Messaging channel allows you to display a message when the user is active within the mobile application. This channel requires mobile applications to be integrated with Adobe Experience Platform SDK.

This tutorial will explain the steps required to set up the mobile properties, the launch extension for the In-App Messaging channel, as well as how to prepare, customize, and send In-App Messages in Adobe Campaign Standard.

## Pre-requisites {#prerequisites}

1. Make sure you can access the **In-App** channel. If you cannot access these channels, contact your account team.  
2. Verify that your **user** has the necessary **permissions** in Adobe Campaign Standard and Launch.

    1. In Adobe Campaign Standard, ensure that the IMS user is part of the Standard User and Administrator groups.  
       This step allows the user to log in to Adobe Campaign Standard, navigate to the Experience Platform SDK mobile app page, and view the mobile app properties that you created in Launch.
    2. In Launch, ensure that your IMS user is part of a Launch product profile.  
       This step allows the user to log in to Launch to create and view the properties. For more information about product profiles in Launch, see [Create your product profile](https://docs.adobelaunch.com/launch-reference/administration/user-permissions#3-create-your-product-profile). In the product profile, there should be no permissions set on the company or the properties, but the user should be able to still log in.

3. In **Adobe Launch:**

    1. create the mobile application by creating a mobile property and instrument your mobile app with Experience Platform SDK.
    2. Install the **Adobe Campaign Standard** extension for your mobile application

For more on extensions, refer to the [Configure Campaign Standard Extension in Launch](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-campaign-standard) in Adobe Launch documentation.

## Steps to Set Up In-App Messages

1. [Configure a mobile application using Adobe Experience Platform SDK](/help/acs/communication-channels/mobile/configure-mobile-apps-using-aep-sdk.md)

2. [Configure Events](/help/acs/communication-channels/mobile/in-app/configure-events.md)

## Create, manage, publish, and report on In-App Deliveries

You have the option to target your users through different delivery templates:

1. [**Broadcast an In-App message**](/help/acs/communication-channels/mobile/in-app/broadcast-in-app-message.md) to target all users of a mobile app

2. **Target all users based on their mobile app profile**
Target all known and/or unknown users (those who have browsed the app in an anonymous mode) with message personalized with user attributes obtained from m This delivery template is geared towards a mixed user base of some known and some anonymous profiles. So, the personalization strategy is based on what you have learnt about the users from their interaction with the device (e.g. target all users who have who have launched their App more than 5 times in last one week).

3. [**Target users based on their Campaign profile**](/help/acs/communication-channels/mobile/in-app/target-users-based-on-campaign-profil.md)
Target known mobile app users (those who have logged into the app with PII) with message personalized with CRM profile attributes available in Campaign. This template is most useful to support cross-channel orchestration use cases, where you have already targeted users on other channels like Email or Push and based on their response, you want to engage them with an in-app message.
4. [Create an In-App delivery within a workflow](/help/acs/communication-channels/mobile/in-app/in-app-activity.md)
5. [Report on your In-App delivery](/help/acs/communication-channels/mobile/in-app/in-app-reporting.md)

## Additional Resources

* [In-App Report (documentation)](https://helpx.adobe.com/campaign/standard/reporting/using/in-app-report.html)
* [Set up a mobile property  (Adobe Launch documentation)](https://aep-sdks.gitbook.io/docs/getting-started/create-a-mobile-property)
* [Configuring a mobile application using Adobe Experience Platform SDKs (documentation)](https://helpx.adobe.com/campaign/kb/configuring-app-sdk.html)
* [Preparing and sending an In-App message (documentation)](https://helpx.adobe.com/campaign/standard/channels/using/preparing-and-sending-an-in-app-message.html)
* [Customizing an In-App message (documentation)](https://helpx.adobe.com/campaign/standard/channels/using/customizing-an-in-app-message.html)
* [Sending an In-App message within a workflow  (documentation)](https://helpx.adobe.com/campaign/standard/automating/using/in-app-delivery.html)
* [Enable Lifecycle Metrics (documentation)](https://aep-sdks.gitbook.io/docs/getting-started/initialize-the-sdk#enable-lifecycle-metrics)
