# Extra Bug Reports (Week 2)

> Note: Screenshots are stored separately in the `Screenshots` folder. PDF contains text only.

## BR-007 — Permanent Address overflow breaks layout in results section
**Reported:** 2026-01-06 14:22
**URL:** https://demoqa.com/text-box
**Environment:** Windows 11, Chrome (latest), Desktop
**Preconditions:** Page is loaded successfully.

**Steps to Reproduce:**
1. Navigate to https://demoqa.com/text-box
2. Enter any valid Full Name and Email
3. Paste 30+ words (or a very long string) into Permanent Address
4. Click Submit

**Expected Result:** The results section renders the submitted address with proper wrapping and consistent spacing without breaking layout.
**Actual Result:** The results section overflows/expands unexpectedly; long text breaks alignment and readability.
**Severity:** Medium
**Priority:** Medium
**Attachment:** Screenshots\Bug_07_UI_Overflow.png
**Notes:** Issue impacts readability and layout stability for long user input.

---

## BR-008 — Multiple client-side resource load failures shown in Console (410 Gone / DNS resolution)
**Reported:** 2026-01-11 10:47
**URL:** https://demoqa.com/text-box
**Environment:** Windows 11, Chrome (latest), Desktop
**Preconditions:** DevTools is available.

**Steps to Reproduce:**
1. Open https://demoqa.com/text-box
2. Open DevTools → Console
3. Reload the page (Ctrl+R)
4. Observe errors/warnings in Console

**Expected Result:** Page resources load successfully; Console contains no critical resource-load errors.
**Actual Result:** Console shows repeated 'Failed to load resource' errors including 410 (Gone) and net::ERR_NAME_NOT_RESOLVED.
**Severity:** High
**Priority:** Medium
**Attachment:** Screenshots\Bug_08_ConsoleErrors.png
**Notes:** May indicate broken third‑party integrations or misconfigured resource endpoints; increases noise and may impact features relying on these resources.

---

## BR-009 — Severe layout shift / misalignment on wide viewport
**Reported:** 2026-01-17 18:33
**URL:** https://demoqa.com/text-box
**Environment:** Windows 11, Chrome (latest), Desktop (wide monitor)
**Preconditions:** Browser window can be resized to very wide width.

**Steps to Reproduce:**
1. Open https://demoqa.com/text-box
2. Resize the browser window to a very wide viewport (e.g., 1800px+ width)
3. Observe the page layout and content positioning

**Expected Result:** Content remains centered/consistent; side elements do not push primary content off-screen.
**Actual Result:** Content shifts far to the right; layout becomes unbalanced and usability decreases on wide viewports.
**Severity:** Medium
**Priority:** Medium
**Attachment:** Screenshots\Bug_09_LayoutShift.png
**Notes:** Likely related to responsive/container rules and/or ad/sidebar layout constraints.

---

## BR-010 — Inconsistent error handling: failing request returns 200 OK with error message in body
**Reported:** 2026-01-20 12:55
**URL:** N/A (Observed during exploratory testing)
**Environment:** Windows 11, Chrome (latest), DevTools Network tab
**Preconditions:** Network tab is open; a failing request can be triggered (e.g., invalid payload / missing parameter).

**Steps to Reproduce:**
1. Open DevTools → Network
2. Trigger a known failing request (e.g., submit invalid input or simulate an unavailable endpoint)
3. Inspect the response status code and body

**Expected Result:** Failure responses return appropriate HTTP error codes (4xx/5xx) with clear error payload.
**Actual Result:** Server responds with 200 OK while the response body contains an error message (failure encoded as success).
**Severity:** High
**Priority:** High
**Attachment:** None
**Notes:** This pattern breaks client error handling, monitoring/alerting, and can cause false positives in automation.

---
