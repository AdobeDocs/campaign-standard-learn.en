---
title: Getting started with Push Notifications with Android App
seo-title: Getting started with Push Notifications with Android App
description: Part 3 - Register mobile extensions 
seo-description: Part 3 - Register mobile extensions
feature: Push
topics: Channels
kt: KT-3846
doc-type: tutorial
activity: use
team: TM
---

# Register Extensions with your mobile app

In this part we will add the code to register the UserProfile,Identity,Lifecycle and Signal extensions. These extensions are part of [Mobile Core Extensions](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/mobile-core). We will also need to register the Campaign extension as shown in the code below.

Open your project in Android studio. Delete the entire code in MainApp **except the first line which is your package statement**
Paste the following code into MainApp

```java{.line-numbers}
import android.app.Application;
import android.util.Log;

import com.adobe.marketing.mobile.AdobeCallback;
import com.adobe.marketing.mobile.Campaign;
import com.adobe.marketing.mobile.Identity;
import com.adobe.marketing.mobile.InvalidInitException;
import com.adobe.marketing.mobile.Lifecycle;
import com.adobe.marketing.mobile.LoggingMode;
import com.adobe.marketing.mobile.MobileCore;
import com.adobe.marketing.mobile.Signal;
import com.adobe.marketing.mobile.UserProfile;

public class MainApp extends Application {

@Override
public void onCreate() {
super.onCreate();

MobileCore.setApplication(this);
MobileCore.setLogLevel(LoggingMode.DEBUG);

try{
    Campaign.registerExtension();
    UserProfile.registerExtension();
    Identity.registerExtension();
    Lifecycle.registerExtension();
    Signal.registerExtension();
    MobileCore.start(new AdobeCallback () {
        @Override
        public void call(Object o) {
            MobileCore.configureWithAppID("copy your launch property id here");
        }
    });
} catch (InvalidInitException e) {
    Log.d("ACS Exception", "exception");
}
}
}

```

Line 32 you need to provide your Launch Property's environment file id. This can be accessed from the environment tab of your launch property.
![launch-id](assets/launch-id-property.PNG)
