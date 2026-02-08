# BR-006 — Category Filter Returns Incorrect Results

**Severity:** High  
**Priority:** High  
**Status:** Open  
**Component:** Filters / Catalog

---

## Summary
Filter displays unrelated products after selecting a specific category.

---

## Description
Selecting a filter (e.g., “Laptops”) returns results from unrelated categories such as “Keyboards” or “Bags”.
This breaks navigation logic and leads to failed product discovery.

---

## Steps to Reproduce
1. Go to Catalog.
2. Select any category filter.
3. Observe the product list.

---

## Expected Result
Only products from the selected category should be displayed.

---

## Actual Result
Mixed or unrelated items appear.

---

## Evidence
- Screenshot: `Filter_Wrong_Results.png`
