---
title: Step 1 - Creating Android App and configuring to use Firebase Cloud Messaging
description: In this part we will create [!DNL Android] App to receive [!UICONTROL Push notifications] sent from Adobe Campaign Standard. In order to receive the push notifications, the app needs to be registered with Google's [!DNL Firebase Cloud Service].
feature: Push
user: Admin
level: Experienced
jira: KT-4825
doc-type: tutorial
activity: use
team: TM
recommendations: noDisplay
exl-id: f087d9f2-cce9-4903-977f-3c5b47522c06
TQID: 'https://experienceleague.adobe.com/-r-0ZHCJNt6bwarH4I-RzA46Ho9EJgDegCnN6VJVLgk'
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
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Step 1 - Creating [!DNL Android] App and configuring to use [!DNL Firebase Cloud Messaging]

In this part you will create [!DNL Android] App to receive [!UICONTROL Push notifications] sent from Adobe Campaign Standard. To receive the push notifications, the app needs to be registered with Google's [!DNL Firebase Cloud Service].

1. Login to your [!DNL Firebase] account.
   
    [!DNL Firebase] is Google's mobile platform that helps you quickly develop high-quality apps. If you do not have a [!DNL Firebase] account, please create one [from here](https://firebase.google.com).

2. Launch [!DNL Android Studio]
3. Click **[!UICONTROL File]** > **[!UICONTROL New]** > **[!UICONTROL New Project].**
4. Select **[!UICONTROL Empty Activity]** and click **[!UICONTROL Next].**

    ![android-project](assets/android-project.PNG)

5. Provide a meaningful name to the project.

   For the purpose of this demo we have named our project as *[!DNL ACSPushTutorial]*

   ![android-project-configuration](assets/android-project-configuration.PNG)

6. Accept the default package names and click **[!DNL Finish]** to create your project.
7. Your project structure should look similar to the screen shot below

    ![android-project-structure](assets/android-project-structure.PNG)

8. Click **[!UICONTROL Tools]** > **[!UICONTROL Firebase].** (this adds the project to [!DNL Firebase])
9. Click **[!UICONTROL Set up Firebase Cloud Messaging].**

    ![setup firebase](assets/android-project-firebase-messaging.PNG)

10. Click **[!UICONTROL Connect to Firebase].**
11. After your app is connected to Firebase, click **[!UICONTROL Add FCM to your app].**
12. Click **[!UICONTROL Accept Changes].**

    When you are adding FCM to your app, the wizard needs your permission to make some changes to your project.

    ![[!DNL add-fcm-to-your-app]](assets/firebase-add-fcm-to-app.PNG)

On successful integration of your app with Firebase, you should get a message like the one shown below:

 ![[!DNL fcm-successfull]](assets/android-firebase-success.PNG)

[Make sure your project is listed in [!DNL Firebase ]console](https://console.firebase.google.com/)

## Configure [!UICONTROL Push Channel] Settings

1. Login to [!DNL Firebase] console
2. Open the **[!UICONTROL ACSPushTutorial]** project.
3. Click the **gear icon** and open the project settings

    ![project-settings](assets/firebase-project-settings.PNG)

4. Tab to the **[!UICONTROL Cloud Messaging]** tab. 
5. Copy the server key

    ![server-key](assets/firebase-server-key.PNG)

6. Login to your Adobe Campaign Standard instance
7. Click **[!UICONTROL Adobe Campaign]** > **[!UICONTROL Administration]** > **[!UICONTROL Channels]** > **[!UICONTROL Mobile App].**
8. Select the appropriate **[!UICONTROL Mobile Application Property].**
9. Click the **[!DNL Android] icon** in the **[!UICONTROL Push Channel settings]** section.
10. Paste the server key in the server key field.

If everything goes well you should see a SUCCESS message.

![push-channel-settings](assets/push-channel-settings.PNG)

To summarize, we have created an [!DNL Android App] and connected the [!DNL Android App] with [!DNL Firebase]. We then connected the Mobile App in Adobe Campaign with the [!DNL Android App] by pasting the [!DNL Android] App's server key in to the Mobile App in Adobe Campaign Standard.
