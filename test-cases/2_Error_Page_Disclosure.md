# Error Page Information Disclosure

## Description
The application displays internal server or application details when an error occurs. Improper error handling may expose sensitive technical information.

## Test Steps
1. Open the application URL.
2. Modify the URL with invalid inputs.
3. Trigger invalid requests or unavailable pages.
4. Observe the error page response.

## Expected Issue
The error page displays:
- Stack traces
- Database errors
- Server paths
- Framework or application details

## Risk
Attackers can gather information about the application's backend structure and technologies, helping them perform targeted attacks.

## Mitigation
- Use custom error pages.
- Disable debug mode in production.
- Avoid displaying internal error details to users.
- Log errors securely on the server side.

## Tools Used
- Burp Suite
- Browser Developer Tools
- OWASP ZAP

## Severity
Medium to High
