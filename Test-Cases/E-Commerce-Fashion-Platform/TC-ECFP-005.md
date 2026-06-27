### TC-ECFP-005: Exhausted Promo Code Restraints
* **Description:** Verify expired or exhausted promo code application restrictions.
* **Preconditions:** A promo code ("WELCOME") exists with an active quantity database configuration set to 0.

| Step | Action | Expected Result |
| :--- | :--- | :--- |
| 1 | Add valid products to the cart and go to Checkout. | Cart total is calculated at standard rate. |
| 2 | Locate the "Promo Code / Voucher" input field. | Input field accepts text. |
| 3 | Enter code "WELCOME" and click "Apply". | Code is rejected; error message appears; order total remains unchanged. |
