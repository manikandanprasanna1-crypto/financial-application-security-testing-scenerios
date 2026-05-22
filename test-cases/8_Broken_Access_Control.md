# Broken Access Control

## Description
The application allows users to access protected pages or resources without proper authentication or authorization.

## Test Steps
1. Login to the application.
2. Copy internal application URLs.
3. Logout from the application.
4. Paste copied URLs directly into browser.
5. Check whether pages are accessible without login.

## Expected Issue
Protected pages or sensitive information are accessible without authentication.

## Risk
- Unauthorized access
- Sensitive data exposure
- Privilege escalation

## Mitigation
- Implement proper authentication checks.
- Validate user sessions properly.
- Apply role-based access control.

## Tools Used
- Browser
- Burp Suite
- OWASP ZAP

## Severity
Critical
