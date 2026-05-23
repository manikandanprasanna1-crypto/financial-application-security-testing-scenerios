# Lack of Transaction PIN Re-Authentication

## Description
The application allows users to perform sensitive financial transactions without requesting password, PIN, or secondary authentication again during the final transaction confirmation step.

## Test Steps
1. Login to the application.
2. Navigate to money transfer or payment section.
3. Enter large transaction amount and recipient details.
4. Proceed to final confirmation step.
5. Verify whether the application asks for:
   - Transaction PIN
   - Password
   - OTP
   - Biometric verification

## Expected Issue
The application completes high-value transactions without asking for re-authentication.

## Risk
- Unauthorized money transfers
- Financial fraud
- Account misuse on unlocked devices
- Increased impact of session hijacking

## Mitigation
- Require transaction PIN or password confirmation for sensitive actions.
- Implement OTP verification for high-value transactions.
- Apply risk-based authentication for critical operations.

## Tools Used
- Manual Testing
- Burp Suite
- OWASP ZAP

## Severity
High to Critical
