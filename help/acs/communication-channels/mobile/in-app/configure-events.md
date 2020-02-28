---
title: Configuring Events
seo-title: Configuring Events
description: When configuring an In-App message in Adobe Campaign Standard (ACS) events define which user initiated action will trigger the message to be displayed. 
feature: In-App
topics: Mobile
kt: 1911
doc-type: feature video
activity: use
team: TM
---

# Configuring Events {#configuring-events}

When configuring an In-App message you need to define which user initiated action will trigger the message to be displayed. These actions are called events. Three categories of events are available: Mobile Application events, Life Cycle events, and Analytics events.

## Mobile Application Events {#mobile-application-events}

Mobile Application events are custom events that are implemented in your mobile application.

Examples are:

* A customer has viewed an item
* A customer adds an item to the cart
* Cart abandonment
* A customer has purchased something

You will need to configure these events in Adobe Campaign. The video below describes how to do this.

>[!VIDEO](https://video.tv.adobe.com/v/26245?quality=12)
*In-App channel-specific application configuration in Adobe Campaign*

## Life Cycle Events  {#life-cycle-events}

Lifecycle events are out-of-the-box events. The following events are available:

* launched
* upgraded
* crashed

An example use case could be a message introducing new features after an upgrade, or an event promotion.

>[!NOTE]
>
>The Lifecycle module needs to be configured in the mobile application. Please see here for more information on [how to add Lifecycle to your app](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/mobile-core/lifecycle)

## Analytics Events {#analytics-events}

The following three categories are supported depending on what is instrumented in your mobile app:

* Adobe Analytics
* Context data
* View state.

>[!NOTE]
>
>Analytics events require an Adobe Analytics licence. Once you have the [Analytics extension configured](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-analytics#configure-analytics-extension-in-launch) and have added [Analytics to your App](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-analytics#add-analytics-to-your-app), these events become available in the In-App configuration in ACS.

## Additional Resources

* [Enable Lifecycle Metrics (documentation)](https://aep-sdks.gitbook.io/docs/getting-started/initialize-the-sdk#enable-lifecycle-metrics)
