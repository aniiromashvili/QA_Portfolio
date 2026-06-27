# BUG-ECFP-005 : Order placement succeeds with blank mandatory address fields when changing country dropdown

## Environment
* **Environment:** Production (Staging Simulated)
* **OS:** Microsoft Windows 11 Pro
* **Browser:** Google Chrome (64-bit)
* **Device:** Desktop
* **Reproducibility Rate:** 100%

## Severity / Priority
* **Severity:** High
* **Priority:** Medium

## Description
The checkout form's client-side validation matrix breaks down when switching destination countries. If a user populates all mandatory fields, changes the "Country" dropdown menu option, and clears the now-incompatible city/street inputs, the system fails to re-trigger blank field validation, allowing an incomplete checkout request to process successfully.

## Steps to Reproduce
1. Navigate to the E-Commerce platform landing page and log in.
2. Add a product to the cart and proceed to the Checkout page.
3. Choose "Home Delivery" and fill out all mandatory shipping details.
4. Change the selection in the "Country" dropdown menu to a different location.
5. Clear the text inside the mandatory "City" and "Street Address" text boxes, leaving them completely empty.
6. Click the "Place Order" / "Proceed to Payment" button.

## Expected Result
The system must block the form submission, display mandatory field validation errors beneath the empty fields, and prevent order creation until valid text is entered.

## Actual Result
The system completely bypasses validation, accepts the blank form parameters, and creates a successful order log with empty shipping destination rows.
