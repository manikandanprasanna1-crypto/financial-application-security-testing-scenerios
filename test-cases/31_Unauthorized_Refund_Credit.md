# Unauthorized Refund Credit

## Description
The application credits refunds without verifying transaction ownership.

## Test Steps
1. Capture refund request.
2. Modify transaction identifiers.
3. Submit request.
4. Verify refund processing.

## Expected Issue
Refund is credited for another user's transaction.

## Risk
- Financial fraud
- Unauthorized credits

## Mitigation
- Verify refund ownership.
- Validate refund eligibility.

## Tools Used
- Burp Suite
- Postman

## Severity
Critical
