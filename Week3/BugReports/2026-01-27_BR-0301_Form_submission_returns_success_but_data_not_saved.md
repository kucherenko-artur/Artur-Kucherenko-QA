# Bug Report

**ID:** BR-0301
**Title:** Form submission returns success but data not saved
**Severity:** major
**Priority:** high
**Status:** New

## Environment
- OS: Windows 11
- Browser: Chrome
- Build/URL: http://127.0.0.1:5500/signup.html

## Preconditions
- Local test page opened

## Steps to reproduce
1. Fill required fields with valid data
2. Click Submit
3. Refresh page

## Expected result
Data is saved and visible after refresh (or confirmation reflects saved record).

## Actual result
Success message appears, but refresh shows no saved data.

## Evidence
- Console/Network: Network tab shows 204 No Content; no storage update in Application tab.
- Screenshot: (add later)

## Notes
Could be missing POST call or backend stub.
