# Session Termination After Password Change

## Description
The application should immediately terminate all active user sessions after a successful password change to prevent unauthorized access using old sessions.

## Test Steps
1. Login to the application.
2. Open another browser or device and login using the same account.
3. Change the account password from one session.
4. Return to the other active session.
5. Try accessing sensitive pages or perform transactions.

## Expected Issue
The previously active session remains valid even after the password has been changed.

## Risk
- Session hijacking
- Unauthorized account access
- Compromised accounts remain accessible

## Mitigation
- Invalidate all active sessions after password change.
- Require users to login again using the new password.

## Tools Used
- Browser
- Burp Suite

## Severity
High
