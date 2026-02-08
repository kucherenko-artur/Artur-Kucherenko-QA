# Bug Report #1
**Reported:** 2026-01-12 13:18
**Title:** reCAPTCHA callback not initialized

**Steps to Reproduce:**
- Open https://demoqa.com/text-box
- Fill valid data
- Open Console
- Submit form

**Expected Result:** reCAPTCHA loads without JS errors
**Actual Result:** Console error: `reCAPTCHA couldn't find user-provided function: onloadCallback`
**Severity:** High
**Priority:** High

---

# Bug Report #2
**Reported:** 2026-01-14 10:41
**Title:** AMP Ads script conflict

**Steps to Reproduce:**
- Open page
- Open Console
- Reload page

**Expected Result:** Ads scripts load once
**Actual Result:** Console: `Ad.Plus-300x250 not requested`, `Format already created`
**Severity:** Medium
**Priority:** Low

---

# Bug Report #3
**Reported:** 2026-01-18 16:55
**Title:** JS crash: setup is not a function

**Steps to Reproduce:**
- Open page
- Inspect Console
- Interact with elements

**Expected Result:** No JS runtime errors
**Actual Result:** Console: `Uncaught TypeError: c(...).setup is not a function`
**Severity:** Critical
**Priority:** Medium

---

# Bug Report #4
**Reported:** 2026-01-21 11:03
**Title:** Missing Interstitial API

**Steps to Reproduce:**
- Open page
- Reload
- Check Console

**Expected Result:** Interstitial API available
**Actual Result:** Console: `vignette: no interstitial API`
**Severity:** High
**Priority:** Low

---

# Bug Report #5
**Reported:** 2026-01-22 15:42
**Title:** Permanent Address layout breaks

**Steps to Reproduce:**
- Open page
- Enter long text
- Submit

**Expected Result:** Text wraps properly
**Actual Result:** Text overflows container
**Severity:** Medium
**Priority:** Medium

---

# Bug Report #6
**Reported:** 2026-01-25 19:28
**Title:** UI Splitter Layout Misalignment

**Steps to Reproduce:**
- Open UI
- Resize window
- Use splitter

**Expected Result:** Splitter maintains layout
**Actual Result:** Panels overlap
**Severity:** High
**Priority:** Medium

---

