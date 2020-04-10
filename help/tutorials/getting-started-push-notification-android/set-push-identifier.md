---
title: STEP 4 - Set pushidentifier
description: The **pushIdentifier** is a string that contains the device token for push notifications. This is the same token that is sent by Firebase and is passed  to the SDK using the MobileCore.setPushIdentifier method.
feature: Push
topics: MOBILE
kt: 4828
doc-type: tutorial
activity: use
team: TM
---
# Step 4 - Set [!DNL pushidentifier]

The **[!DNL pushidentifier]** is a string that contains the device token for [!DNL Push] notifications. This is the same token that is sent by [!DNL Firebase] and is passed to the SDK using the [!DNL MobileCore.setPushIdentifier] method.

Open your project in [!DNL Android ]studio. Delete the entire code in [!DNL MainActivity] **except the first line which is your package statement**.

Paste the following code into [!DNL MainActivity]:

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

* Run your app by clicking green arrow or select **[!DNL Run->Run'app']**.
* The [!DNL Android] emulator should start and you should see your app running with [!DNL "Hello World" ]text.
* Open the [!DNL logcat] window. Search for "[!DNL Got]". You should see the token that was received from [!DNL Firebase] written to the log as shown below. The long string after "[!DNL Got token]" is the [!DNL pushidentifier ]that is sent to Adobe Campaign.

![logcat-token](assets/logcat-got-token.PNG)

### Check Mobile Application Subscribers

Login to your Adobe Campaign Standard instance.
Navigate **[!UICONTROL Administration->Channels->Mobile App(AEP SDK)]**. Open the appropriate mobile application. Tab to the [!UICONTROL Mobile Application Subscribers] tab. You should see a [!UICONTROL registration token ]listed.

![mobile-application-subscribers](assets/mobile-application-subscribers.PNG)

>[NOTE]
>If you do not see registration token in the [!UICONTROL Mobile Application Subscribers] tab STOP here before proceeding any further.
