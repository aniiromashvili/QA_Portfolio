# BUG-ECFP-001 : Expired promo code is successfully applied and deducts order total

## Environment
* **Environment:** Production (Staging Simulated)
* **OS:** Microsoft Windows 11 Pro
* **Browser:** Google Chrome (64-bit)
* **Device:** Desktop
* **Reproducibility Rate:** 100%

## Severity / Priority
* **Severity:** High
* **Priority:** High

## Description
During the checkout process, the system allows the application of an expired/exhausted promotional voucher ("WELCOME"). The system accepts the voucher code and deducts the discount value from the total order cost, despite the voucher balance/quantity configuration being set to 0 in the system logic.

## Steps to Reproduce
1. Navigate to the E-Commerce platform landing page.
2. Log in with valid user credentials.
3. Add products to the shopping cart to reach a total value exceeding 250 GEL.
4. Proceed to the Checkout page.
5. Input the promotional voucher code "WELCOME" into the promo code field and apply it.
6. Observe the order breakdown summary and system response.

## Expected Result
The system must reject the promo code and display an appropriate validation error message. The order total should remain unchanged since the voucher availability count is 0.

## Actual Result
The system successfully validates and applies the exhausted voucher, deducting 50 GEL from the total order balance, completely bypassing the zero-quantity inventory limitation.
