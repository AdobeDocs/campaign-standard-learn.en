---
title: Part 6 - Send Push notification to test your work
description: Part 6 - Send Push notification to test your work
feature: Push
jira: KT-4830
user: Admin
level: Experienced
doc-type: tutorial
activity: use
team: TM
exl-id: 10218e1f-6e85-490a-84d9-c5d42bd2321d
TQID: 'https://experienceleague.adobe.com/NrQc40vzqTy0fNfVT6fN0IjMKuXjilt6eZV-lgZpAcQ'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: f5407121-8933-4ac3-8e06-a9b692a4e88a
    internal-label: Campaign Standard
feature_v2:
  - id: a4671286-a59f-47e3-b97b-90627a1977d5
    internal-label: Communication channels
subfeature_v2:
  - id: a4657621-810c-498b-8a27-7ced9c176dda
    internal-label: Push notifications
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
---
# Part 6 - Send [!UICONTROL Push Notification] to test your work

We now need to create and send a [!UICONTROL Push Notification] using Adobe Campaign. To create a simple push notification for testing purposes, please follow the following steps.

* Log in to your Adobe Campaign Standard instance
* Click **[!UICONTROL Marketing Activities]->[!UICONTROL Create]->[!UICONTROL Push Notification]**
* Select **[!UICONTROL Send push to app subscribers(mobileApp)]** and click Next
* Select the appropriate mobile app from the **[!UICONTROL Associate a Mobile App to a delivery]** drop-down list and click **[!UICONTROL Next]**
* Click the count label and it should return a value greater than 0. Click **[!UICONTROL Next]**
* Provide a meaningful [!UICONTROL Message title] and [!UICONTROL Message body] and click **[!UICONTROL Create]**.
* Click **[!UICONTROL Prepare]**. Once preparation, is complete click **[!UICONTROL Confirm]** to send the message.

If everything goes well, you should see notification in your Android&trade; App running in the emulator

## Additional resources

* [Detailed documentation on Push Notifications](https://experienceleague.adobe.com/docs/campaign-standard/using/communication-channels/push-notifications/about-push-notifications.html?lang=en)
* [Creating a Push Notification(Video)](/help/communication-channels/mobile/push-notifications/creating-a-push-notification.md)
