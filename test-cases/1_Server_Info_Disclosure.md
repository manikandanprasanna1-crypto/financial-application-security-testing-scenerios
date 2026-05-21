# Server Information Disclosure

## Description
The website exposes server information in HTTP headers.

## Test Steps
1. Open the website
2. Inspect response headers
3. Check Server and X-Powered-By headers

## Expected Issue
Server details are visible.

## Risk
Attackers can identify vulnerable technologies.

## Mitigation
Hide unnecessary server details.

## Tools Used
- Burp Suite
- Browser DevTools

## Severity
Medium
