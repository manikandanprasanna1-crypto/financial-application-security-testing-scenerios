# Password Reset Link Expiration

## Description
The application allows password reset links to remain valid for a long duration.

## Test Steps
1. Request password reset link.
2. Wait for extended time period.
3. Attempt to use the same reset link again.
4. Verify whether the link still works.

## Expected Issue
Password reset links remain active beyond secure time limits.

## Risk
Attackers can reuse old reset links to compromise accounts.

## Mitigation
- Expire reset links within short duration.
- Invalidate links after single use.

## Tools Used
- Burp Suite
- Browser

## Severity
High
