How to check debug mode enabled

Debug mode is a feature that allows developers to debug and test their apps on an Android device. When enabled, debug mode can allow an 
attacker to gain access to sensitive information and perform other malicious actions on the device.

Steps to check for insecure Android permissions for debug mode enabled:

1. Obtain a copy of the APK file for the Android app that you want to check for insecure Android permissions.

2. Use a tool such as Apktool or Jadx to decompile the APK file and view the app's AndroidManifest.xml file.

3. Check if the app uses android:debuggable="true" in the AndroidManifest.xml file.

4. Check if the app uses any anti-debugging mechanism to prevent debug mode from being enabled.

5. Check if the app uses any anti-tampering mechanism to prevent the app from being modified.

6. Check if the app uses any root detection mechanism to prevent the app from running on rooted devices.

7. Check if the app uses any function that checks for the presence of the android.permission.SET_DEBUG_APP permission.

8. Check if the app uses any function that checks for the presence of the android.os.Debug.isDebuggerConnected() method.
