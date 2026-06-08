# Receiver Account Substitution

## Description
The application allows modification of the beneficiary account during transaction processing.

## Test Steps
1. Initiate a fund transfer.
2. Capture the request.
3. Change beneficiary account details.
4. Forward the request.
5. Verify transaction destination.

## Expected Issue
Funds are transferred to an unauthorized account.

## Risk
- Unauthorized fund transfer
- Financial fraud

## Mitigation
- Validate beneficiary details server-side.
- Digitally sign transaction requests.

## Tools Used
- Burp Suite
- OWASP ZAP

## Severity
Critical
