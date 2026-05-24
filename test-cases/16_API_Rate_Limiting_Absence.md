# API Rate Limiting Absence on Balance Checks

## Description
The application does not restrict the number of API requests sent to the balance check endpoint, allowing attackers to send excessive requests continuously.

## Test Steps
1. Login to the application.
2. Identify the balance check API endpoint.
3. Send repeated requests rapidly using automated tools.
4. Observe server response time and application behavior.

## Expected Issue
The application allows unlimited API requests without blocking or throttling excessive traffic.

## Risk
- Server slowdown or denial of service
- Resource exhaustion
- Poor performance for legitimate users
- Increased infrastructure load

## Mitigation
- Implement API rate limiting.
- Restrict number of requests per user/IP.
- Use throttling and request monitoring.
- Apply CAPTCHA or temporary blocking for abnormal traffic.

## Tools Used
- Burp Suite Intruder
- Postman
- JMeter
- OWASP ZAP

## Severity
High
