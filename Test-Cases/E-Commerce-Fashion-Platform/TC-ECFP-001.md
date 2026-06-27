### TC-ECFP-001: Checkout Delivery Matrix Restrictions
* **Description:** Verify delivery options matrix for "Online Only" products during checkout.
* **Preconditions:** User is logged in; an item flagged as "Online Only" is identified.

| Step | Action | Expected Result |
| :--- | :--- | :--- |
| 1 | Navigate to the PDP of the "Online Only" product. | Product details page loads successfully. |
| 2 | Add the item to the shopping cart. | Product is added; cart counter updates. |
| 3 | Proceed to the Checkout page. | Checkout form and shipping options are rendered. |
| 4 | Expand the Delivery Methods section. | **In-Store Pickup** is disabled/hidden. Only **Home Delivery** is selectable. |
