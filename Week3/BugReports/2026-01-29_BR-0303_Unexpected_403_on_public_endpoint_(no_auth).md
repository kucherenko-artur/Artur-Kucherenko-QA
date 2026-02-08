# Bug Report

**ID:** BR-0303
**Title:** Unexpected 403 on public endpoint (no auth)
**Severity:** major
**Priority:** medium
**Status:** New

## Environment
- OS: Windows 11
- Browser: Chrome
- Build/URL: https://example.com/api/public

## Preconditions
- No auth headers set

## Steps to reproduce
1. Open DevTools
2. Send GET request to /api/public
3. Observe response

## Expected result
200 OK with public payload.

## Actual result
403 Forbidden returned.

## Evidence
- Console/Network: Response headers show auth middleware triggered.
- Screenshot: (add later)

## Notes
Maybe route incorrectly protected.
