# Password Reset Token Reusability

## Description
The application allows password reset tokens to be reused multiple times.

## Test Steps
1. Request password reset token.
2. Reset password successfully.
3. Attempt to reuse the same token again.
4. Verify whether token is still accepted.

## Expected Issue
Previously used password reset tokens remain valid.

## Risk
Attackers may repeatedly reset passwords using reused tokens.

## Mitigation
- Invalidate tokens immediately after use.
- Generate unique one-time reset tokens.

## Tools Used
- Burp Suite
- OWASP ZAP

## Severity
High
