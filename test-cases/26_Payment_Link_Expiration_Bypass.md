# Payment Link Expiration Bypass

## Description
The application fails to enforce expiration checks on payment links, allowing users to access and use expired payment URLs.

## Test Steps
1. Generate a payment link.
2. Wait until the link expiration time has passed.
3. Open the expired payment link.
4. Attempt to complete a payment.
5. Observe the application response.

## Expected Issue
The expired payment link remains active and accepts payments.

## Risk
- Unauthorized transactions
- Reuse of old payment sessions
- Financial fraud

## Mitigation
- Validate payment link expiry on the server side.
- Invalidate expired links automatically.
- Generate unique one-time payment links.

## Tools Used
- Browser
- Burp Suite
- Postman

## Severity
High
