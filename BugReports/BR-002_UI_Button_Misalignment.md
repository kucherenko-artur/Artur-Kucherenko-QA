# BR-002 —BR-00X — Secure Page Accessible via Browser Back After Logout

Severity: High  
Severity Justification: High severity because a previously authenticated secure page remains accessible after logout via browser back navigation. This indicates improper session invalidation or missing cache-control headers, potentially exposing sensitive information to unauthorized users.
Status: Open  
Component: UI / Layout  
Environment: Windows 11, Chrome 121

---

## Summary
After logging out, the protected /secure page can still be accessed using the browser Back button without re-authentication.

---

## Description
A layout shift occurs in the product page card. The button is slightly lower than the product rating and price elements.
This creates a visual imbalance, making the UI look inconsistent.

---

## Steps to Reproduce
1. Open: https://the-internet.herokuapp.com/login
2. Enter valid credentials:
   - Username: tomsmith
   - Password: SuperSecretPassword!
3. Click **Login**.
4. Confirm the "Secure Area" page is displayed with message:
   "You logged into a secure area!"
5. Open **Browser Console (F12)** and observe console errors.
6. Click **Logout**.
7. Click the browser **Back** button.
8. Observe that the "Secure Area" page content is displayed again.
9. Press **Refresh (F5)**.
10. Observe red message:
    "You must login to view the secure area!"

## Expected Result
After logout, protected content must not be accessible.
Using the browser Back button should not display the Secure Area page content.

## Actual Result
After clicking Back, the Secure Area page content is temporarily displayed (likely from browser cache).
After refreshing the page, access is denied and user is redirected to Login Page.

## Severity
Informational

## Severity Justification
There is no real security bypass — access is correctly denied after page refresh.
However, displaying protected content after logout (via browser cache) may cause confusion and represents a potential UX/security concern.

## Evidence

### 1. Login Page – Credentials Entered
![Login Page – Credentials Entered](../../assets/BR-002/BR-002_LoginPage_Credentials_Filled.png)

---

### 2. Secure Area – Successful Login
![Secure Area – Successful Login](../../assets/BR-002/BR-002_SecureArea_SuccessLogin.png)

---

### 3. Secure Area – Console Errors Visible
![Secure Area – Console Errors Visible](../../assets/BR-002/BR-002_SecureArea_Console_Errors.png)

---

### 4. Login Page – After Logout
![Login Page – After Logout](../../assets/BR-002/BR-002_LoginPage_AfterLogout.png)

---

### 5. Access Denied Message After Refresh
![Access Denied Message](../../assets/BR-002/BR-002_LoginPage_AccessDenied_Message.png)

