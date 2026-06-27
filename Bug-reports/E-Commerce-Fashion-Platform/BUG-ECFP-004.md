# BUG-ECFP-004 : Cart total allows negative pricing when reducing item quantity below zero via API modification

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
The shopping cart total value logic fails to enforce server-side validation against negative bounds. If an item quantity parameter is manually altered or manipulated to a negative integer (e.g., -1) during the cart updating phase, the system recalculates the final order balance backwards, resulting in a negative total amount.

## Steps to Reproduce
1. Navigate to the E-Commerce platform landing page.
2. Log in with valid user credentials.
3. Add any product to the shopping cart.
4. Navigate to the Shopping Cart view.
5. Intercept or manipulate the quantity update request (or use input manipulation) to set the product count to a negative value.
6. Observe the updated shopping cart total and summary fields.

## Expected Result
The system must reject negative integers for product quantities, returning a validation error. The cart quantity should defaults to a minimum value of 1 or completely remove the item.

## Actual Result
The system accepts the negative value, subtracts the item cost from the total balance, and renders a negative total price (e.g., -45 GEL) on the screen.
