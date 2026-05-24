# Insecure Data Storage in Mobile Cash Apps

## Description
The mobile application stores sensitive user information such as bank account numbers, card details, or personal data in plaintext format within the device’s local storage.

## Test Steps
1. Install and login to the mobile application.
2. Perform normal application activities.
3. Access the device local storage or application data directory.
4. Check files, databases, shared preferences, or cache storage.
5. Verify whether sensitive information is stored in readable format.

## Expected Issue
Sensitive user information such as bank account numbers or personal data is stored in plaintext within local device storage.

## Risk
- Sensitive data theft
- Privacy compromise
- Financial fraud
- Unauthorized access to confidential information

## Mitigation
- Encrypt sensitive data before local storage.
- Avoid storing confidential information unnecessarily.
- Use secure mobile storage mechanisms such as Android Keystore or iOS Keychain.

## Tools Used
- Android Studio Device Explorer
- ADB
- MobSF
- Frida

## Severity
Critical
