### Test Case ID: TC-ACW-002 – Verify AI Chatbot Context Boundary Enforcement
* **Related Bug:** BUG-001
* **Module:** AI Chat Framework
* **Type:** Security / Boundary Test
* **Priority:** Critical
* **Precondition:**
  * The user has access to multiple project boards with active and inactive states.
  * Inactive boards contain distinct structural assets, YouTube references, and localized Georgian text.
* **Steps:**
  1. Access the active workspace interface.
  2. Open the AI Chat Panel and initiate a query regarding the current board layout.
  3. Inspect the response payload and generated text for any cross-contamination or background data leaks.
* **Expected Result:**
  * The system must reject data queries attempting to pull background metadata from unrelated project environments.
  * Response content must remain strictly bound to the active view state parameters.
