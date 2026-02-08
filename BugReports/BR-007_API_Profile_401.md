# BR-007 — Profile API Returns 401 for Logged-In User

**Severity:** Critical  
**Priority:** High  
**Status:** Open  
**Component:** API / Authentication

---

## Summary
Authenticated user receives 401 Unauthorized from `/profile` endpoint.

---

## Description
Even while logged in, an API call to `/api/profile` responds with 401.
This blocks the user from accessing personal data and breaks session logic.

---

## Steps to Reproduce
1. Log into account.
2. Open DevTools → Network.
3. Refresh the page.
4. Inspect `/api/profile` request.

---

## Expected Result
API returns 200 OK with JSON user profile.

---

## Actual Result
API returns 401 Unauthorized.

---

## Evidence
- Screenshot: `Profile_API_401.png`
