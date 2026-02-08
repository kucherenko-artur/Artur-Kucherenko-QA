# Bug Report

**ID:** BR-0105
**Title:** Search suggestions dropdown doesn't populate
**Severity:** major
**Priority:** high
**Status:** New

## Environment
- OS: Windows 11
- Browser: Chrome
- Build/URL: https://www.amazon.ca

## Preconditions
- User is on homepage
- Network is available

## Steps to reproduce
1. Open homepage
2. Click search field
3. Type `abc`
4. Wait 3 seconds

## Expected result
Suggestion list appears under the search field.

## Actual result
Suggestion area stays blank; spinner flashes; request fails intermittently.

## Evidence
- Console/Network: Network tab shows request to suggestions endpoint returning 500/timeout.
- Screenshot: (add later)

## Notes
Observed more often after page refresh; may be caching/session related.
