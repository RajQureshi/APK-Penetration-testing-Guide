To check for sensitive information in local storage on an Android device, you can use the following steps:

1. Connect the device to your computer and enable USB debugging.

2. Open a command prompt or terminal window and navigate to the platform-tools folder in the Android SDK directory.

3. Use the command adb shell to access the device's command line.

4. Use the command run-as <your.package.name> to switch to the app's sandbox.

5. Use the command ls -al to list all files in the app's local storage directory.

6. Inspect the files and directories for any sensitive information such as passwords, tokens, or keys. Alternatively, you can use a command such as find /data/data/<your.package.name> -type f -exec grep -H "password" {} \; to search for specific keywords in all the files of the app's local storage directory.

