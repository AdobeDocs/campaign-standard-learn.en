---
title: Getting started with Push Notifications with Android App
seo-title: Getting started with Push Notifications with Android App
description: Part 1 - Creating your Android App and adding to Firebase. 
seo-description: Part 1 - Creating your Android App and adding to Firebase
feature: Push
topics: Channels
kt: KT-3846
doc-type: tutorial
activity: use
team: TM
---

# Creating Android App and Configuring to use Firebase Cloud Messaging

In this part we will create Android App to receive push notifications sent from Adobe Campaign Standard.In order to receive the push notifications, app needs to be registered with Google's Firebase Cloud Service.

1. Login to your Firebase account. Firebase is Google's mobile platform that helps you quickly develop high-quality apps. If you do not have Firebase account, please create one [from here](https://firebase.google.com).
1. Launch Android Studio
1. Click on File -> New -> New Project
1. Select Empty Activity and click Next

  ![android-project](assets/android-project.PNG)

1. Provide a meaningful name to the project. For the purpose of this demo we have named our project as "ACSPushTutorial"
 
 ![android-project-configuration](assets/android-project-configuration.PNG)

1. Accept the default package names and click on Finish to create your project.
1. Your project structure should look similar to the screen shot below
 
  ![android-project-structure](assets/android-project-structure.PNG)

1. Click on Tools ->Firebase(This adds the project to Firebase)
1. Click on Set up Firebase Cloud Messaging
    
  ![setup firebase](assets/android-project-firebase-messaging.PNG)


1. Click on **Connect to Firebase**
1. After your app is connected to Firebase, click on **Add FCM to your app**
1. When you are adding FCM to your app the wizard will need your permission to make some changes to your project.Click on **Accept Changes**

 ![add-fcm-to-your-app](assets/firebase-add-fcm-to-app.PNG)
1. On successful integration of your app with Firebase, you should get a message like shown below
 ![fcm-successfull](assets/android-firebase-success.PNG)
1. [Make sure your project is listed in Firebase console](https://console.firebase.google.com/)

## Configure Push Channel Settings

1. Login to Firebase console
1. Open the **ACSPushTutorial** project. Click on the gear icon and open the project settings 

![project-settings](assets/firebase-project-settings.PNG)

1. Tab to the **Cloud Messaging** tab. Copy the server key

![server-key](assets/firebase-server-key.PNG)

1. Login to your Adobe Campaign Standard instance
1. Click on Adobe Campaign -> Administration->Channels->Mobile App
1. Select the appropriate Mobile Application Property
1. Click on the Android icon in the Push Channel settings section
1. Paste the server key in the Server key field. Everything goes well you should see a SUCCESS message.

![push-channel-settings](assets/push-channel-settings.PNG)

To summarize, we have created Android App and connected the Android App with Firebase. We then connected the Mobile App with the Android App by pasting the Android App's server key in to the Mobile App in Adobe Campaign Standard.
