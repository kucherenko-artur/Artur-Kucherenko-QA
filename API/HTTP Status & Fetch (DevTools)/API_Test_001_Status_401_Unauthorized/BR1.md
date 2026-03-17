# API Test — HTTP 401 Unauthorized

## Purpose
Verify how the browser and Fetch API behave when requesting an endpoint that requires authentication.

## Request Details
- **Endpoint:** https://httpbin.org/basic-auth/user/passwd
- **Tool:** Chrome DevTools (Console / Network)
- **Method:** GET

## Expected Result
- Server returns **401 Unauthorized** when credentials are not provided.
- Browser may display a **Basic Authentication prompt**.

## Actual Result
- Response status: **401 Unauthorized**
- Browser displays a login/password prompt.

## Evidence
See screenshots in the `evidence/` folder.

## Notes
Training API test created for QA portfolio demonstration using DevTools.
