# API Test — HTTP 500 Internal Server Error

## Purpose
Verify how DevTools and Fetch handle **server-side errors (5xx responses)**.

## Request Details
- **Endpoint:** https://httpbin.org/status/500
- **Tool:** Chrome DevTools (Console / Network)
- **Method:** GET

## Expected Result
- Response status: **500 Internal Server Error**
- Error visible in DevTools console or network logs.

## Actual Result
- Console shows **500 Internal Server Error**
- Status code visible via response inspection.

## Evidence
Screenshots available in the `evidence/` folder.

## Notes
Example of handling server-side failures during API testing.
