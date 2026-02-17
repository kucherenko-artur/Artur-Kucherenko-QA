# BR-001 — Search Suggestions Not Displayed Correctly

**Severity:** High  
**Priority:** High  
**Status:** Open  
**Component:** Search  
**Environment:**  
- OS: Windows 11  
- Browser: Chrome 121  
- Date: 2026-02-07

---

## Summary
Search suggestions fail to appear or appear with significant delay during input.

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
