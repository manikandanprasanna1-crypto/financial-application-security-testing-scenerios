# SSL/TLS Certificate Validation

## Description
The application uses expired, invalid, or insecure SSL/TLS configuration.

## Test Steps
1. Open the HTTPS website.
2. Click the lock icon near the browser URL.
3. Check:
   - Certificate validity
   - Expiry date
   - TLS version
   - Certificate issuer

## Expected Issue
- Expired SSL certificate
- Invalid certificate
- Weak TLS versions are used

## Risk
- Man-in-the-Middle (MITM) attacks
- Data interception
- Untrusted communication

## Mitigation
- Renew SSL certificates regularly.
- Use TLS 1.2 or TLS 1.3.
- Disable weak protocols and ciphers.

## Tools Used
- SSL Labs
- OpenSSL
- Browser

## Severity
High
