# Recurring Payment Modification

## Description
The application allows users to alter recurring payment schedules without proper authorization.

## Test Steps
1. Create a recurring payment.
2. Intercept modification requests.
3. Change amount or frequency.
4. Submit request.

## Expected Issue
Recurring payment details are modified without proper verification.

## Risk
- Unauthorized recurring charges
- Financial abuse

## Mitigation
- Require authentication for modifications.
- Validate ownership of recurring payments.

## Tools Used
- Burp Suite
- Postman

## Severity
High
