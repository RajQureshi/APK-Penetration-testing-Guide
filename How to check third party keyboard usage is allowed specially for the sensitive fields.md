How to check Third party keyboard enabled for the third party keyboard usage is allowed specially for the sensitive fields step by step

Third-party keyboard usage can be a security concern as they may collect sensitive information entered by users. It's important to ensure that third-party keyboard usage is allowed only for non-sensitive fields and that the app has appropriate controls in place to prevent sensitive information from being leaked.

Steps to check for third-party keyboard usage for sensitive fields:

1. Obtain a copy of the APK file for the Android app that you want to check for third-party keyboard usage.

2. Use a tool such as Apktool or Jadx to decompile the APK file and view the app's source code.

3. Inspect the source code for any fields that accept sensitive information, such as password fields or credit card fields.

4. Check if the app uses any controls to prevent third-party keyboard usage for sensitive fields, such as disabling the use of third-party keyboards for specific fields.

5. Inspect the codebase for any calls to the following class:
InputMethodManager

6. Check if the app uses any encryption algorithm to encrypt the sensitive data before sending to the third-party keyboard.

7. Test the app by using a third-party keyboard and check if sensitive information is being sent to the third-party keyboard.


how to check Third party keyboard enabled for the third party keyboard usage is allowed specially for the sensitive fields step by step using adb


Steps to check for third-party keyboard usage for sensitive fields using ADB:

1. Connect your android device to your computer

2. Open command prompt and navigate to the platform-tools folder in the android sdk

3. Run the command "adb shell dumpsys input_method" to list all the input methods installed on the device

4. Look for the third-party keyboard you want to test

5. Open the app you want to test and go to the sensitive field, such as a password field or credit card field

6. Try to input sensitive information using the third-party keyboard

7. Observe if the sensitive information is being sent to the third-party keyboard

8. Check if the app uses any encryption algorithm to encrypt the sensitive data before sending to the third-party keyboard.
