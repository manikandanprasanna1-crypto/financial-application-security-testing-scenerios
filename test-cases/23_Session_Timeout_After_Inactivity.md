# Session Timeout After Inactivity

## Description
The application does not automatically log out users after a period of inactivity.

## Test Steps
1. Login to the application.
2. Leave the session idle for the configured timeout period.
3. Attempt to access application pages without re-authentication.
4. Verify whether the session remains active.

## Expected Issue
The session remains active even after long periods of inactivity.

## Risk
Unauthorized users may access active sessions on unattended devices.

## Mitigation
- Configure automatic session timeout.
- Force re-authentication after inactivity.
- Invalidate inactive sessions on the server side.

## Tools Used
- Browser
- Burp Suite

## Severity
Medium
