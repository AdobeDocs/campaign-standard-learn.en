---
title: Getting started with Push Notifications with Android App
seo-title: Getting started with Push Notifications with Android App
description: Part 6 - Send push notification to test your work
seo-description: Part 6 - Send push notification to test your work
feature: Push
topics: Channels
kt: KT-3846
doc-type: tutorial
activity: use
team: TM
---

# Create Push Notification

We now need to create and send push notification using Adobe Campaign. [Detailed documentation on push notification](https://docs.adobe.com/content/help/en/campaign-standard/using/communication-channels/push-notifications/about-push-notifications.html). To create a simple push notification for testing purposes, please follow the following steps.

* Login to your Adobe Campaign Standard instance
* Click on **Marketing Activities->Create->Push Notification**
* Select **Send push to app subscribers(mobileApp)** and click Next
* Select the appropriate mobile app from the **Associate a Mobile App to a delivery** drop down list and click **Next**
* Click on the Count label and it should return a value greater than 0. Click Next
* Provide a meaningful Message title and Message body and click Create.
* Click on Prepare. Once preparation, is complete click on Confirm to send the message.
* If everything goes well, you should see notification in your Android App running in the emulator
