# Sensitive Data Exposure

## Description
The application exposes sensitive information such as passwords, tokens, personal details, or confidential data in plaintext format instead of encrypting it.

## Test Steps
1. Open the application.
2. Login using valid credentials.
3. Intercept requests and responses.
4. Check whether sensitive information is visible in readable format.
5. Verify whether HTTPS encryption is enabled.

## Expected Issue
Sensitive data such as passwords, session IDs, or personal information is visible in plaintext.

## Risk
- Data theft
- Identity theft
- Credential compromise
- Unauthorized access

## Mitigation
- Use HTTPS/TLS encryption.
- Encrypt sensitive information.
- Hash passwords securely.
- Avoid storing confidential data in plaintext.

## Tools Used
- Burp Suite
- Wireshark
- Browser Developer Tools

## Severity
Critical
