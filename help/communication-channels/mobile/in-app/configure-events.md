---
title: Configure Events
description: "Understand how events define which user initiated action will trigger an in-app message to be displayed. "
feature: In App
kt: 2548
thumbnail: 26245.jpg
doc-type: feature video
activity: use
team: TM
exl-id: 2c7937f4-b0da-46e5-934e-c660012c2c6f
role: Business Practitioner, Developer
level: Beginner, Intermediate
---
# Configure [!UICONTROL Events] {#configuring-events}

When configuring an [!UICONTROL In-App] message, you need to define which user-initiated action triggers the message to be displayed. These actions are called [!UICONTROL events]. Three categories of [!UICONTROL events] are available: [!UICONTROL Mobile Application events], [!UICONTROL Life Cycle events], and [!UICONTROL Analytics events].

## [!UICONTROL Mobile Application Events] {#mobile-application-events}

[!UICONTROL Mobile Application events] are [!UICONTROL custom events] that are implemented in your mobile application.

Examples are:

* A customer has viewed an item
* A customer adds an item to the cart
* Cart abandonment
* A customer has purchased something

You must configure these [!UICONTROL events] in Adobe Campaign. The following video describes how to do this.

>[!VIDEO](https://video.tv.adobe.com/v/26245?quality=12)

## [!UICONTROL Life Cycle events]  {#life-cycle-events}

[!UICONTROL Lifecycle events] are out-of-the-box [!UICONTROL events]. The following [!UICONTROL events] are available:

* [!UICONTROL launched]
* [!UICONTROL upgraded]
* [!UICONTROL crashed]

An example use case could be a message introducing new features after an upgrade, or an event promotion.

>[!NOTE]
>
>The [!UICONTROL Lifecycle module] needs to be configured in the mobile application. Please see here for more information on [How to add Lifecycle to your app](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/mobile-core/lifecycle)

## [!UICONTROL Analytics Events] {#analytics-events}

The following three categories are supported depending on what is instrumented in your mobile app:

* Adobe Analytics
* [!UICONTROL Context data]
* [!UICONTROL View state]

>[!NOTE]
>
>[!UICONTROL Analytics events] require an Adobe Analytics license. Once you have the [[!DNL Analytics] extension configured](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-analytics#configure-analytics-extension-in-launch) and have added [Analytics to your App](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-analytics#add-analytics-to-your-app), these events become available in the [!UICONTROL In-App] configuration in ACS.

## Additional resources

* [Enable Lifecycle Metrics (documentation)](https://aep-sdks.gitbook.io/docs/getting-started/initialize-the-sdk#enable-lifecycle-metrics)
