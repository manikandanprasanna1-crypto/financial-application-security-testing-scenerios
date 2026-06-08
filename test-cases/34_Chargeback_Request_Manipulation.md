# Chargeback Request Manipulation

## Description
The application allows users to submit or modify chargeback requests without proper validation of transaction ownership or eligibility.

## Test Steps
1. Login to the application.
2. Navigate to transaction history.
3. Select a completed transaction.
4. Intercept the chargeback request.
5. Modify transaction identifiers or chargeback parameters.
6. Submit the modified request.
7. Verify whether the chargeback is accepted.

## Expected Issue
The application processes unauthorized or manipulated chargeback requests.

## Risk
- Financial fraud
- Revenue loss
- Unauthorized refunds
- Dispute process abuse

## Mitigation
- Verify transaction ownership.
- Validate chargeback eligibility.
- Implement approval workflows for chargebacks.
- Log and monitor chargeback requests.

## Tools Used
- Burp Suite
- Postman
- OWASP ZAP

## Severity
Critical
