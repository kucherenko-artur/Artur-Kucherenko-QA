# API Test — HTTP 204 No Content

## Purpose
Verify that the server correctly returns **204 No Content** and does not include a response body.

## Request Details
- **Endpoint:** https://httpbin.org/status/204
- **Tool:** Chrome DevTools (Console / Network)
- **Method:** GET

## Expected Result
- Response status: **204 No Content**
- Response body is empty.

## Actual Result
- Console shows **Status: 204**
- No response body returned.

## Evidence
Screenshots available in the `evidence/` folder.

## Notes
Basic API validation test for HTTP status handling.
