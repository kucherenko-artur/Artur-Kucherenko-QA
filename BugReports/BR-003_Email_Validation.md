# BR-003 — Email Field Accepts Invalid Format

Severity: Medium  
Severity Justification: The issue does not block form submission, but it allows invalid user data to be stored, which may impact communication and system data integrity.  
**Priority:** High  
**Status:** Open  
**Component:** Form Validation  
**Environment:** Chrome 121, Windows 11

---

## Summary
The email validation allows submission of malformed addresses, potentially leading to invalid user data in the system.

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

### Impact

- Users may not receive notifications or confirmation emails.
- Account recovery flows may fail.
- Invalid email data may be stored in the database, affecting data integrity.

---

## Evidence
- Screenshot: `Email_Validation_Issue.png`
