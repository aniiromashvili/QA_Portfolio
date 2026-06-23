### Test Case ID: TC-ACW-006 – Verify Feature Parity and Model Selector Consistency across Views
* **Related Bug:** BUG-005
* **Module:** AI Chat Panel
* **Type:** Functional Consistency Test
* **Priority:** Medium
* **Precondition:**
  * The user has an active project workspace with accessible Draft and Board view modules.
* **Steps:**
  1. Open the workspace and navigate into the Draft view state.
  2. Open the AI Chat Panel and inspect the available model selector options and features.
  3. Switch the workspace layout directly to the active Board view state.
  4. Open the AI Chat Panel again and compare the model selector parameters against the Draft view baseline.
* **Expected Result:**
  * Complete feature parity must be maintained across both application perspectives.
  * The model selector dropdown options must match identically between the Draft and Board view configurations with no missing UI components.
