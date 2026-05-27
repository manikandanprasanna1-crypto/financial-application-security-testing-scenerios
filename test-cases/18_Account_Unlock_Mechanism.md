# Account Unlock Mechanism

## Description
The application does not provide a secure mechanism to unlock accounts after multiple failed login attempts.

## Test Steps
1. Trigger account lock using multiple failed logins.
2. Verify available account unlock methods.
3. Check whether identity verification is required.

## Expected Issue
Accounts can be unlocked insecurely or without proper verification.

## Risk
Unauthorized users may regain account access.

## Mitigation
- Use secure identity verification.
- Require OTP or email verification before unlocking.

## Tools Used
- Manual Testing
- Burp Suite

## Severity
Medium to High
