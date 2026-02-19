# BR-003 — Forgot Password Returns 500 Internal Server Error

**Severity:** Critical (S1)

**Severity Justification:**  
The “Forgot Password” functionality is a core authentication feature. If the system responds with a 500 Internal Server Error during a password reset attempt, users are blocked from regaining access to their accounts. There is no workaround available, and this directly affects security, account accessibility, and system reliability. Because the issue breaks a critical authentication flow and prevents legitimate users from logging in, severity is classified as **Critical (S1)**.

**Priority:** High (P1)

**Priority Justification:**  
Password reset issues directly affect user access and support workloads. A 500 server error must be fixed before release to ensure account recovery works reliably and does not generate customer lockouts. Therefore, priority is classified as **High (P1)**.

**status:** Open

---

## Summary

Submitting the "Forgot Password" form results in a **500 Internal Server Error**, indicating a backend failure instead of proper validation or user feedback.

---

## Description

When a user attempts to reset their password via the "Forgot Password" functionality, the system responds with a 500 Internal Server Error.

This indicates:
- Missing backend error handling
- Possible unhandled exception
- Improper validation or missing configuration

A password recovery feature is a critical authentication component and must not return server errors.

---

## Steps to Reproduce

1. Open https://the-internet.herokuapp.com/login  
2. Click **"Forgot Password"**  
3. Enter any email address  
4. Click **Retrieve password**

---

## Expected Result

The system should:
- Display a confirmation message (e.g., "Password reset email sent")
OR
- Validate input and return a controlled error message

The page must not return a server error.

---

## Actual Result

The page returns:

**500 Internal Server Error**

Network tab confirms:
- Request Method: POST
- Endpoint: /forgot_password
- Status Code: 500

---

## Impact

- Password recovery is unusable
- Authentication flow is broken
- Indicates backend instability
- Damages system reliability perception

---

## Evidence

### 1. Internal Server Error Page
![Internal Server Error](../Evidence/Raw/BR-003_01_Forgot_Password_Internal_Server_Error.png)

### 2. Network Tab – 500 Status
![Network 500](../Evidence/Raw/BR-003_02_Network_Request_500.png)

### 3. Request Headers – POST /forgot_password (500)
![Headers 500](../Evidence/Raw/BR-003_03_Request_Headers_500.png)
