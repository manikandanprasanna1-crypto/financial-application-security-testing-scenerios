# Password Reuse Restriction

## Description
The application allows users to reuse previously used passwords during password changes.

## Test Steps
1. Login to the application.
2. Change the password.
3. Attempt to reuse an old password.
4. Verify whether the application accepts it.

## Expected Issue
Previously used passwords are accepted again.

## Risk
Compromised old passwords may continue to be reused, reducing account security.

## Mitigation
- Maintain password history.
- Restrict reuse of previous passwords.

## Tools Used
- Manual Testing
- Burp Suite

## Severity
Medium
