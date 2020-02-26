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
# Set push identifier

**pushIdentifier** is a string that contains the device token for push notifications. This is the same token that is sent by Firebase and is passed  to the SDK using the MobileCore.setPushIdentifier method.

Open your project in Android studio. Delete the entire code in MainActivity **except the first line which is your package statement**
Paste the following code into MainActivity

```java{.line-numbers}
import androidx.annotation.NonNull;
import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.util.Log;
import android.widget.Toast;

import com.adobe.marketing.mobile.MobileCore;
import com.google.android.gms.tasks.OnCompleteListener;
import com.google.android.gms.tasks.Task;
import com.google.firebase.iid.FirebaseInstanceId;
import com.google.firebase.iid.InstanceIdResult;

public class MainActivity extends AppCompatActivity {

@Override
protected void onCreate(Bundle savedInstanceState) {
super.onCreate(savedInstanceState);
setContentView(R.layout.activity_main);

registerToken();
}

void registerToken() {
FirebaseInstanceId.getInstance().getInstanceId()
    .addOnCompleteListener(new OnCompleteListener<InstanceIdResult>() {
        @Override
        public void onComplete(@NonNull Task<InstanceIdResult> task) {
            if (!task.isSuccessful()) {
                Log.w("Message App", "getInstanceId failed", task.getException());
                return;
            }

// Get new Instance ID token
String token = task.getResult().getToken();

Log.d("Got token", token);

MobileCore.setPushIdentifier(token);
}
});
}

@Override
public void onResume() {
super.onResume();
MobileCore.setApplication(getApplication());
MobileCore.lifecycleStart(null);
}

@Override
public void onPause() {
super.onPause();
MobileCore.lifecyclePause();
}
}

```

## Test your app

Now is a good time to test your app, before going any further.

* Run your app by clicking green arrow or select Run->Run'app'
* The Android emulator should start and you should see your app running with "Hello World" text.
* Open the logcat window.Search for "Got". You should see the token that was received from firebase written to the log as shown below.The long string after "Got token" is the push identifier that is sent to Adobe Campaign
![logcat-token](assets/logcat-got-token.PNG)

### Check Mobile Application Subscribers

Login to your Adobe Campaign Standard instance
Navigate Administration->Channels->Mobile App(AEP SDK). Open the appropriate mobile application. Tab to the Mobile Application Subscribers tab. You should a registration token
![mobile-application-subscribers](assets/mobile-application-subscribers.PNG)

>[NOTE]
>If you do not see registration token in the Mobile Application Subscribers tab STOP here before proceeding any further.
