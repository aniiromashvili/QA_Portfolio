### TC-ECFP-003: Cart Quantity Zero-Bound Validation
* **Description:** Verify cart behavior when a single product's quantity is updated to zero.
* **Preconditions:** User is logged in; at least one item is present in the shopping cart.

| Step | Action | Expected Result |
| :--- | :--- | :--- |
| 1 | Navigate to the Shopping Cart page. | Cart items and total breakdown are displayed. |
| 2 | Locate the product quantity input field. | Input field is editable. |
| 3 | Manually type `0` into the input and press Enter. | System prompts deletion modal or automatically removes item. Cart total updates cleanly. |
