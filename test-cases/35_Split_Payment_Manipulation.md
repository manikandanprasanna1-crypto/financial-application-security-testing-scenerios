# Split Payment Manipulation

## Description
The application allows users to manipulate payment distribution when a transaction amount is split between multiple merchants, vendors, or beneficiaries.

## Test Steps
1. Initiate a split payment transaction.
2. Intercept the payment request.
3. Modify beneficiary allocation amounts.
4. Forward the request.
5. Verify how the payment is distributed.

## Expected Issue
The application accepts modified allocation values and distributes funds incorrectly.

## Risk
- Unauthorized fund diversion
- Financial fraud
- Incorrect settlement processing
- Merchant disputes

## Mitigation
- Calculate split allocations on the server side.
- Validate beneficiary distribution before processing.
- Digitally sign settlement requests.

## Tools Used
- Burp Suite
- Postman
- OWASP ZAP

## Severity
Critical
