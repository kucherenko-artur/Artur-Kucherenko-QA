# API Test — HTTP 302 Redirect (Follow)

## Purpose
Demonstrate how browsers automatically follow **302 redirects** and how the final response differs from the initial redirect.

## Request Details
- **Endpoint:** https://httpbin.org/status/302
- **Tool:** Chrome DevTools (Console / Network)
- **Method:** GET

## Expected Result
- Initial request returns **302 Found**
- Response contains **Location header**
- Browser follows redirect automatically
- Final request returns **200 OK**

## Actual Result
- Console displays final status **200 OK**
- Network panel shows redirect chain:
  - 302 Found
  - Location header
  - Follow-up request → 200 OK

## Evidence
Screenshots located in the `evidence/` folder:
- Console output
- Network request list
- Redirect headers

## Notes
Demonstrates redirect chains and how browsers process them.
