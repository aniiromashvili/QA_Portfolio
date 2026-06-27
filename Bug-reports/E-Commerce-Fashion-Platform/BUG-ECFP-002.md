# BUG-ECFP-002 : 'In-Store Pickup' option is available for 'Online Only' products

## Environment
* **Environment:** Production (Staging Simulated)
* **OS:** Microsoft Windows 11 Pro
* **Browser:** Google Chrome (64-bit)
* **Device:** Desktop
* **Reproducibility Rate:** 100%

## Severity / Priority
* **Severity:** Medium
* **Priority:** Medium

## Description
During the checkout phase, the system provides the "In-Store Pickup" (physical branch collection) delivery option even when the shopping cart contains items explicitly flagged and designated as "Online Only". The checkout delivery matrix fails to dynamically restrict or filter out warehouse-bound inventory options based on product availability restrictions.

## Steps to Reproduce
1. Navigate to the E-Commerce platform landing page.
2. Log in with valid user credentials.
3. Search for and select a product designated exclusively as an "Online Only" item.
4. Navigate to the Product Detail Page (PDP) to confirm its exclusive online availability status.
5. Add the product to the shopping cart and proceed to the Checkout page.
6. Observe the available delivery methods section.

## Expected Result
The "In-Store Pickup" option must be hidden or disabled on the Checkout page when an "Online Only" product is in the cart. Only direct home delivery should be selectable.

## Actual Result
Both "Home Delivery" and "In-Store Pickup" options remain fully available and selectable, completely ignoring the product's online-exclusive restriction.
