### TC-ECFP-002: Dynamic Branch Filtering
* **Description:** Verify dynamic filtering of physical branches based on stock availability.
* **Preconditions:** User is logged in; a product available at only 2 specific branches is in the cart.

| Step | Action | Expected Result |
| :--- | :--- | :--- |
| 1 | Proceed to the Checkout page. | Checkout page loads successfully. |
| 2 | Select "In-Store Pickup" as the delivery method. | Branch selection dropdown menu becomes active. |
| 3 | Click and expand the branch selection dropdown. | System displays **only the 2 branches** where the item is actively in stock. |
