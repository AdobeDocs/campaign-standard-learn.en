---
title: Introduction to In-App messages
description: Learn how to present the user with contextually relevant in-app messages in response to a customer's real-time behavior within the mobile application.
feature: In App
kt: 1911
doc-type: feature video
activity: use
team: TM
exl-id: c51716eb-7239-4fc0-9ccf-9f5f0a5fae65
role: User
level: Beginner
---
# Introduction to [!UICONTROL In-App] messages {#introduction}

The [!UICONTROL In-App Messaging] channel allows you to display a message when the user is active within the mobile application. This channel requires mobile applications to be integrated with [!UICONTROL Adobe Experience Platform SDK].

This tutorial explains the steps required to set up the mobile properties, the [!UICONTROL Launch] extension for the [!UICONTROL In-App Messaging] channel, and how to prepare, customize, and send [!UICONTROL In-App] messages in Adobe Campaign Standard. The links lead to the video tutorials on each of the highlighted topics.

## Prerequisites {#prerequisites}

1. Make sure you can access the **[!UICONTROL In-App]** channel. If you cannot access these channels, contact your account team.  
1.  Verify that your **user** has the necessary **permissions** in Adobe Campaign Standard and [!UICONTROL Launch].

    1. In Adobe Campaign Standard, ensure that the IMS user is part of the [!UICONTROL Standard User] and [!UICONTROL Administrator] groups.

       This step allows the user to log in to Adobe Campaign Standard, navigate to the Experience Platform SDK mobile app page, and view the mobile app properties that you created in [!UICONTROL Launch].

    1. In [!UICONTROL Launch], ensure that your IMS user is part of a [!UICONTROL Launch] product profile. This step allows the user to log in to [!UICONTROL Launch] to create and view the properties. In the product profile, there should be no permissions set on the company or the properties, but the user should be able to still log in.

1. In Adobe Experience Platform Launch:

    1. Create the mobile application by creating a mobile property and instrument your mobile app with Experience Platform SDK.
    1. Install the **Adobe Campaign Standard** extension for your mobile application.

For more on extensions, refer to [Configure Campaign Standard extension in Adobe Launch](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-campaign-standard) in the documentation.

## Steps to set up [!UICONTROL In-App] messages {#steps-to-set-up}

1. [Configure a mobile application using Adobe Experience Platform SDK](/help/communication-channels/mobile/configure-mobile-apps-using-aep-sdk.md).
1. [Configure events](/help/communication-channels/mobile/in-app/configure-events.md).

## Create, manage, and publish [!UICONTROL In-App] Deliveries {#create-manage-publish}

You can either create one time In-App deliveries by clicking the **[!UICONTROL Create an In-App Message]** card from the homepage, from the [!UICONTROL Marketing Activities], or you can [Create an In-App delivery within a workflow](/help/communication-channels/mobile/in-app/in-app-activity.md).

When setting up the delivery, you have three options to target your users by choosing from different delivery templates:

1. [**Broadcast an In-App message**](/help/communication-channels/mobile/in-app/broadcast-in-app-message.md) to target all users of a mobile app. 

   This message type enables you to send messages to all users (current or future) of your mobile application even if they don't have an existing profile in Adobe Campaign. Personalization is therefore not possible when customizing the messages as the user profile does not necessarily exist in Adobe Campaign.
   
1. Target all users based on their mobile app profile.

   This message type enables you to target all known or anonymous users of a mobile app that have a mobile profile in Adobe Campaign. This messages type can be personalized using only non-personal and non-sensitive attributes and does not require secure handshake between Mobile SDK and Adobe Campaign's In-App messaging service. So, the personalization strategy is based on what you have learned about the users from their interaction with the device. For example target all users who have  launched their App more than five times in last one week.

1. [**Target users based on their Campaign profile**](/help/communication-channels/mobile/in-app/target-users-based-on-campaign-profile.md).

   This message type enables you to target Adobe Campaign profiles (CRM profiles) who have subscribed to your mobile application. The message can be personalized with all available profile attributes in Adobe Campaign. It requires a secure handshake between Mobile SDK and Campaign's In-App messaging service to ensure that messages with personal and sensitive information are used by authorized users only.

This template is useful to support cross-channel orchestration use cases, where you have already targeted users on other channels like Email or Push. Based on their response, you then want to engage them with an In-App message.

## Report on your In-App deliveries {#report}

Once your delivery has been published, you can [report on your In-App delivery](/help/communication-channels/mobile/in-app/in-app-reporting.md).

## Additional resources

* [In-App Report](https://experienceleague.adobe.com/docs/campaign-standard/using/reporting/list-of-reports/in-app-report.html?lang=en)
* [Set up a mobile property](https://aep-sdks.gitbook.io/docs/getting-started/create-a-mobile-property)
* [Configuring a mobile application using Adobe Experience Platform SDKs](https://experienceleague.adobe.com/docs/campaign-standard/using/administrating/configuring-channels/configuring-a-mobile-application.html?lang=en)
* [Preparing and sending an In-App message](https://experienceleague.adobe.com/docs/campaign-standard/using/communication-channels/in-app-messaging/preparing-and-sending-an-in-app-message.html?lang=en)
* [Customizing an In-App message](https://experienceleague.adobe.com/docs/campaign-standard/using/communication-channels/in-app-messaging/customizing-an-in-app-message.html?lang=en)
* [Sending an In-App message within a workflow](https://experienceleague.adobe.com/docs/campaign-standard/using/managing-processes-and-data/channel-activities/in-app-delivery.html?lang=en)
* [Enable Lifecycle Metrics](https://aep-sdks.gitbook.io/docs/getting-started/initialize-the-sdk#enable-lifecycle-metrics)
