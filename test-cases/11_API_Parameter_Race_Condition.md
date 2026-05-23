# API Parameter Race Condition

## Description
The application processes multiple requests simultaneously without proper transaction handling or synchronization. An attacker can send many requests at the same time to exploit delayed balance updates.

## Test Steps
1. Login to the application.
2. Open the money withdrawal or transaction feature.
3. Intercept the API request.
4. Send multiple requests simultaneously using automated tools.
5. Observe account balance and transaction history.

## Expected Issue
The application processes multiple withdrawal requests before updating the balance, allowing users to withdraw more money than available.

## Risk
- Financial fraud
- Balance manipulation
- Unauthorized transactions
- Business logic exploitation

## Mitigation
- Implement transaction locking mechanisms.
- Use atomic database transactions.
- Apply request rate limiting.
- Validate balance before every transaction processing.

## Tools Used
- Burp Suite Intruder
- OWASP ZAP
- Postman
- JMeter

## Severity
Critical
