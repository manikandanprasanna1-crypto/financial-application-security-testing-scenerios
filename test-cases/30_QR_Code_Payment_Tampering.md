# QR Code Payment Tampering

## Description
The application trusts payment details encoded within QR codes without sufficient validation.

## Test Steps
1. Generate payment QR code.
2. Modify encoded payment details.
3. Scan altered QR code.
4. Complete payment.

## Expected Issue
Payment processes using manipulated QR data.

## Risk
- Misdirected payments
- Financial fraud

## Mitigation
- Sign QR payloads digitally.
- Validate payment details on the server.

## Tools Used
- QR Decoder
- Burp Suite

## Severity
Critical
