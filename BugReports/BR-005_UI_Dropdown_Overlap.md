# BR-005 — Dropdown Overlaps Other UI Elements

**Severity:** Low  
**Priority:** Low  
**Status:** Open  
**Component:** UI / Layout

---

## Summary
Dropdown menu overlaps UI elements underneath it, hiding content.

---

## Description
When the dropdown expands, it visually overlaps text or buttons behind it due to missing z-index or padding.

---

## Steps to Reproduce
1. Open any form with a dropdown.
2. Click the dropdown.
3. Observe overlapping sections.

---

## Expected Result
Dropdown should push content downward or layer above cleanly.

---

## Actual Result
Dropdown visually overlaps existing elements.

---

## Evidence
- Screenshot: `Dropdown_Overlap.png`
