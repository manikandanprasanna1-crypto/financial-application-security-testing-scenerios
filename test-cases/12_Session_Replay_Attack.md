# Session Replay in Financial Forms

## Description
The application allows previously completed financial transaction requests to be captured and replayed again, causing duplicate transactions or unauthorized repeated actions.

## Test Steps
1. Login to the application.
2. Perform a money transfer transaction.
3. Intercept the transaction request using a proxy tool.
4. Save the completed request.
5. Replay the same request again.
6. Verify whether the transaction is processed multiple times.

## Expected Issue
The application accepts the previously completed request again and processes duplicate transactions.

## Risk
- Double charging users
- Unauthorized repeated transactions
- Financial fraud
- Transaction manipulation

## Mitigation
- Implement unique transaction IDs.
- Use anti-replay tokens or nonce values.
- Expire transaction requests after completion.
- Validate duplicate requests on the server side.

## Tools Used
- Burp Suite Repeater
- OWASP ZAP
- Postman

## Severity
Critical
