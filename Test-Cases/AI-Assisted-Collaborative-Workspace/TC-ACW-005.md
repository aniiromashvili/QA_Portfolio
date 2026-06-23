### Test Case ID: TC-ACW-005 – Verify Text Object Edit State and Data Retention
* **Related Bug:** BUG-004
* **Module:** Board Workspace Canvas
* **Type:** Functional / Regression Test
* **Priority:** High
* **Precondition:**
  * The user is on the active interactive workspace board layout.
  * At least one text object with pre-existing string content is deployed on the canvas.
* **Steps:**
  1. Navigate to the interactive board canvas.
  2. Execute a single-click action directly on the pre-existing text object to enter the editing state.
  3. Observe the behavior of the text node and the stability of the input field.
* **Expected Result:**
  * The existing text content must remain persistent and intact upon activation of the edit mode.
  * The input field must not auto-wipe or clear data dynamically during selection changes.
