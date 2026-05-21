# Password Autofill Enabled

## Description
The browser automatically stores and fills login credentials on the application login page.

## Test Steps
1. Open the application login page.
2. Enter username and password.
3. Login successfully.
4. Logout from the application.
5. Open the login page again.
6. Check whether username or password is auto-filled.

## Expected Issue
Saved credentials are automatically displayed in the login fields.

## Risk
Anyone using the same device may gain unauthorized access to the account.

## Mitigation
- Disable autocomplete for sensitive fields.
- Encourage use of secure password managers.
- Implement Multi-Factor Authentication (MFA).

## Tools Used
- Browser
- Browser Developer Tools

## Severity
Low to Medium
