# BR-001 — Search Suggestions Not Displayed Correctly

**Severity:** High  
Severity Justification: Core navigation functionality is impacted, directly affecting product discovery and conversion.
**Priority:** High  
**Status:** Open  
**Component:** Search  
**Environment:**  
- OS: Windows 11  
- Browser: Chrome 121  
- Date: 2026-02-07

---

## Summary
Search suggestions either fail to appear or are delayed by 1–3 seconds during input.

---

## Description
When the user types into the search bar, autocomplete suggestions either load too slowly or do not appear at all.
This negatively affects navigation and UX, especially for long queries or mobile users.

---

## Steps to Reproduce
1. Open the website home page.
2. Click on the search input field.
3. Begin typing any product name (e.g., "laptop").
4. Observe the suggestions area.

---

## Expected Result
Suggestions should appear instantly (≤ 150 ms).

---

## Actual Result
Suggestions appear with a noticeable delay (1–3 seconds) or do not appear at all.

---

## Evidence
- Screenshot / Video: `Search_Suggestions_Delay.png`
