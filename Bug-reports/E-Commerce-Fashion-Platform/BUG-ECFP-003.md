# BUG-ECFP-003 : All physical branches are displayed for in-store pickup despite limited product availability

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
When selecting the "In-Store Pickup" delivery option during checkout, the location dropdown filters fail to dynamically validate inventory locations. The system displays all existing physical branches in the network list, even if the selected product in the cart is physically available and in stock at only two specific branches.

## Steps to Reproduce
1. Navigate to the E-Commerce platform landing page.
2. Log in with valid user credentials.
3. Select an item known to have limited stock availability (e.g., physically present in only 2 physical stores).
4. Verify the limited stock locations on the Product Detail Page (PDP).
5. Add the product to the shopping cart and proceed to the Checkout page.
6. Select "In-Store Pickup" as the preferred delivery method.
7. Click on the branch location selection menu and observe the listed stores.

## Expected Result
The system must dynamically filter the store list to only render and display the specific physical branches where the item is actively in stock (in this scenario, only 2 valid locations).

## Actual Result
The system exposes all available company branches in the dropdown list, including locations with zero stock for the selected items.
