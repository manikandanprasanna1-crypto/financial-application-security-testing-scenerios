# Missing Multi-Factor Authentication (MFA)

## Description
The application allows login using only username and password without any second level authentication.

## Test Steps
1. Open the application login page.
2. Login using valid credentials.
3. Verify whether additional authentication is required such as:
   - OTP
   - Authenticator App
   - Biometrics

## Expected Issue
The application allows login without second-factor verification.

## Risk
If user credentials are stolen, attackers can directly access accounts.

## Mitigation
- Implement Multi-Factor Authentication (MFA).
- Use OTP verification.
- Use authenticator applications or biometric verification.

## Tools Used
- Manual Testing
- Burp Suite

## Severity
High
