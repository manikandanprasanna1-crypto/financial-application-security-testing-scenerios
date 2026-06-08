# Transaction Fee Manipulation

## Description
The application allows users to modify transaction fees through request tampering.

## Test Steps
1. Initiate a payment transaction.
2. Intercept the request.
3. Modify transaction fee value.
4. Submit the request.
5. Verify payment processing.

## Expected Issue
Modified fee values are accepted.

## Risk
- Revenue loss
- Financial manipulation

## Mitigation
- Calculate fees on the server side.
- Ignore client-supplied fee values.

## Tools Used
- Burp Suite
- Postman

## Severity
High
