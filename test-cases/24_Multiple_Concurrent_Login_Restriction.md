# Multiple Concurrent Login Restriction

## Description
The application allows the same user account to be logged in from multiple devices or locations simultaneously without restrictions.

## Test Steps
1. Login using User A on Device 1.
2. Login using the same account on Device 2.
3. Perform activities from both devices.
4. Verify whether concurrent sessions are allowed.

## Expected Issue
The application allows unlimited simultaneous active sessions.

## Risk
- Account sharing
- Unauthorized account access
- Session misuse

## Mitigation
- Restrict concurrent logins.
- Notify users about new logins.
- Allow users to terminate active sessions.

## Tools Used
- Browser
- Mobile Device
- Burp Suite

## Severity
Medium
