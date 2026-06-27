# Checklist - E-Commerce Fashion Platform

### Cart Mechanics & Pricing Logic
- [ ] Verify that altering or modifying item quantities in the cart to negative integers is rejected by server-side safeguards.
- [ ] Verify that removing a line item completely recalculates the cart summary block, taxes, and final totals in real-time.
- [ ] Verify that applying an exhausted or expired promo code string explicitly returns a clear error message.

### Checkout Funnel & Branch Constraints
- [ ] Verify that the 'In-Store Pickup' delivery option is automatically hidden or grayed out if the cart contains 'Online Only' products.
- [ ] Verify that the branch pickup menu dropdown lists only the physical locations where the item is actively in stock.
- [ ] Verify that clicking the 'Place Order' button with missing mandatory shipping parameters freezes the action and shows validation errors.
- [ ] Verify that modifying the country selector dynamically updates localized delivery pricing rules and regional input masks.
