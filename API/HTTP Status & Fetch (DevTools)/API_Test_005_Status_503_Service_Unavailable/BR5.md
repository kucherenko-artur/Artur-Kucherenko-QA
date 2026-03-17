# API Test — HTTP 503 Service Unavailable

## Purpose
Verify behavior when the server returns **503 Service Unavailable**.

## Request Details
- **Endpoint:** https://httpbin.org/status/503
- **Tool:** Chrome DevTools (Console / Network)
- **Method:** GET

## Expected Result
- Response status: **503 Service Unavailable**
- Response headers visible in Network tab.

## Actual Result
- Network panel shows **503 Service Unavailable**
- Headers and response metadata available for inspection.

## Evidence
Screenshots stored in the `evidence/` folder.

## Notes
Demonstrates how temporary service failures appear in API testing.
