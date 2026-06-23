### Test Case ID: TC-ACW-001 – Verify Workspace Data Isolation Stability and Context Retention
* **Related Bug:** BUG-001
* **Module:** AI Chat Framework
* **Type:** Functional / Security Test
* **Priority:** High
* **Precondition:**
  * The user environment possesses at least two distinct, isolated project workspaces created (e.g., Workspace A and Workspace B).
  * Each respective workspace contains entirely different visual elements, text configurations, and media nodes on its interactive board.
* **Steps:**
  1. Open the platform URL and navigate into the workspace interface for Workspace A.
  2. Locate and initialize the AI Chat Panel from the upper-right control header.
  3. Submit a direct context-specific prompt to the assistant: "What's on Project1's board?"
  4. Evaluate the validation accuracy of the generated AI text response against the actual visual items present on the active board layout.
* **Expected Result:**
  * The AI assistant must enforce strict workspace isolation and data boundaries.
  * The model must contextually parse, synthesize, and describe only the specific active board metadata that directly correlates with the user's explicit query and active session workspace.
  * No metadata, links, or localized text from Workspace B should be leaked or returned.
