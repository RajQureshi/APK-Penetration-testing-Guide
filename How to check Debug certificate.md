how to check Debug certificate for check if the application is using Debug certificate using keytool step by step

Steps to check for Debug certificate in an Android application using keytool

1. Obtain the APK file of the Android application you want to check.
2. Extract the .apk file to a directory on your computer.
3. Open the command prompt or terminal on your computer.
4. Navigate to the directory where the APK file was extracted.
5. Use the following command to check the certificate:
Copy code
keytool -printcert -file META-INF/CERT.RSA
6. Look for the "CN=Android Debug,O=Android,C=US" in the output, this indicates that the application is using a debug certificate.

Alternatively, 
7. You can use the following command to check the certificate:
Copy code
jarsigner -verify -verbose -certs <apk-file-name>

