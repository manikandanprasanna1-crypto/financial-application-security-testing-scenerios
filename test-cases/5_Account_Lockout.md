# Missing Account Lockout Policy

## Description
The application allows unlimited failed login attempts without temporarily blocking the account.

## Test Steps
1. Open the application login page.
2. Enter incorrect password multiple times.
3. Attempt more than 3–5 failed logins.
4. Check whether the account gets locked or blocked.

## Expected Issue
The account remains active even after multiple failed login attempts.

## Risk
Attackers can perform brute-force or credential stuffing attacks to guess passwords.

## Mitigation
- Implement temporary account lockout.
- Add CAPTCHA after multiple failed attempts.
- Apply rate limiting for login requests.

## Tools Used
- Burp Suite
- Hydra
- OWASP ZAP

## Severity
High
