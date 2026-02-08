# BR-003 — Email Field Accepts Invalid Format

**Severity:** Medium  
**Priority:** High  
**Status:** Open  
**Component:** Form Validation  
**Environment:** Chrome 121, Windows 11

---

## Summary
The email field accepts invalid input formats (missing @ symbol or domain).

---

## Description
User can enter incorrect email formats such as:
- `test`
- `user@mail`
- `@gmail.com`

The system allows form submission without showing validation errors.

---

## Steps to Reproduce
1. Navigate to Registration / Checkout / Profile Update form.
2. Enter an invalid email (e.g., `abc`).
3. Try to submit.

---

## Expected Result
Invalid email formats should be blocked with a clear error message.

---

## Actual Result
Invalid emails are accepted and the form proceeds.

---

## Evidence
- Screenshot: `Email_Validation_Issue.png`
