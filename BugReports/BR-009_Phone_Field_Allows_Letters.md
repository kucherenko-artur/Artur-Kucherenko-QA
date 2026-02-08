# BR-009 — Phone Number Field Accepts Letters

**Severity:** Medium  
**Priority:** High  
**Status:** Open  
**Component:** Form Validation

---

## Summary
Phone Number field incorrectly accepts alphabetic characters.

---

## Description
User can enter letters (`abc`) or mixed characters (`a123b`) in the phone number field.
This allows invalid data to pass through frontend validation.

---

## Steps to Reproduce
1. Open form with phone input.
2. Enter alphabetic characters.
3. Attempt to continue.

---

## Expected Result
Only numeric characters allowed.

---

## Actual Result
Letters are accepted without restrictions.

---

## Evidence
- Screenshot: `Validation_Phone_Allowed_Letters.png`
