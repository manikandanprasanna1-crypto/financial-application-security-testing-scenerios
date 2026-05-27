# Old Password Validation During Password Change

## Description
The application allows users to change passwords without verifying the current password.

## Test Steps
1. Login to application.
2. Navigate to change password page.
3. Attempt password change without entering old password.
4. Verify whether password change succeeds.

## Expected Issue
Application changes password without validating old password.

## Risk
Unauthorized users with temporary session access can change account passwords.

## Mitigation
- Require current password verification before password changes.
- Implement additional re-authentication for sensitive actions.

## Tools Used
- Manual Testing
- Burp Suite

## Severity
High
