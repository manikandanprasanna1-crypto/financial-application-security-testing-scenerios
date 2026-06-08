# Cashback Eligibility Bypass

## Description
Users can receive cashback rewards despite not meeting eligibility criteria.

## Test Steps
1. Perform a non-eligible transaction.
2. Intercept request.
3. Modify reward-related parameters.
4. Complete transaction.

## Expected Issue
Cashback is awarded incorrectly.

## Risk
- Financial loss
- Reward system abuse

## Mitigation
- Calculate rewards server-side.
- Validate eligibility before crediting.

## Tools Used
- Burp Suite
- Postman

## Severity
High
