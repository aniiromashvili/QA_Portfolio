### TC-ECFP-004: Checkout Form State Mutation Validation
* **Description:** Verify mandatory field validation on Checkout form when changing delivery country.
* **Preconditions:** User is on the Checkout page with a product in the cart.

| Step | Action | Expected Result |
| :--- | :--- | :--- |
| 1 | Select "Home Delivery" and fill all mandatory fields. | Form validation flags pass (green state). |
| 2 | Change the "Country" selection dropdown. | Fields persist or clear based on region configuration. |
| 3 | Clear the text from "City" and "Street Address" fields. | Fields are visually empty. |
| 4 | Click the "Place Order" button. | Submission is blocked; inline validation errors appear under blank fields. |
