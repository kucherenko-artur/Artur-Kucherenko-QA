# BR-004 — Cart Quantity Not Updating

**Severity:** High  
**Priority:** High  
**Status:** Open  
**Component:** Cart / Checkout

---

## Summary
Changing product quantity does not update the total price.

---

## Description
When the user modifies product quantity in the cart, total price remains the same until page refresh.
This may cause incorrect order totals and financial inconsistencies.

---

## Steps to Reproduce
1. Add any product to cart.
2. Go to the cart.
3. Change quantity from 1 → 2 or 3.
4. Observe the total amount.

---

## Expected Result
Total price recalculates automatically after quantity changes.

---

## Actual Result
Total price remains unchanged until manual page reload.

---

## Evidence
- Screenshot: BR-004_Cart_Quantity_Not_Updating.png
