# Predictable Transaction IDs

## Description
The application generates transaction IDs or receipt links in a predictable sequential format, allowing users to access other users’ transaction details by modifying the ID value.

## Test Steps
1. Login to the application.
2. Complete a transaction.
3. Observe the transaction receipt URL or transaction ID.
4. Change the transaction ID manually in the URL.
   Example:
   tx_id=5001 → tx_id=5002
5. Check whether another user’s transaction details become accessible.

## Expected Issue
The application allows access to other users’ transaction receipts or sensitive details by modifying transaction IDs.

## Risk
- Unauthorized access to financial records
- Information disclosure
- Privacy violations
- Business logic abuse

## Mitigation
- Use random and unpredictable transaction IDs.
- Implement proper authorization checks.
- Validate ownership of transaction records before displaying data.

## Tools Used
- Burp Suite
- Browser
- OWASP ZAP

## Severity
Critical
