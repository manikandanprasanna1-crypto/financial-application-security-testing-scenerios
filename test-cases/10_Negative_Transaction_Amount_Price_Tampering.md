# Negative Transaction Amounts (Price Tampering)

## Description
The application fails to properly validate transaction amounts. A user can modify the transfer amount in the request from a positive value to a negative value, causing incorrect balance calculations.

## Test Steps
1. Login to the application.
2. Initiate a money transfer transaction.
3. Intercept the request using a proxy tool.
4. Change the transfer amount from:
   100
   to
   -500
5. Forward the modified request.
6. Check account balance and transaction response.

## Expected Issue
The application accepts negative transaction values and incorrectly credits money to the user's account.

## Risk
- Financial fraud
- Unauthorized balance manipulation
- Business logic abuse
- Monetary loss to the organization

## Mitigation
- Validate transaction amounts on the server side.
- Reject negative or invalid values.
- Implement strong business logic validation.
- Apply transaction integrity checks.

## Tools Used
- Burp Suite
- OWASP ZAP
- Postman

## Severity
Critical
