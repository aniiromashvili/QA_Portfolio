### Test Case ID: TC-ACW-003 – Verify AI Chatbot Response Logic and Clarification Prompting
* **Related Bug:** BUG-002
* **Module:** AI Chat Framework
* **Type:** Functional / Usability Test
* **Priority:** Medium
* **Precondition:**
  * The user is inside an active Board Workspace session.
  * The AI Chat interface is open and responsive.
* **Steps:**
  1. Input a vague or incomplete prompt that lacks critical details required to execute a board action.
  2. Execute the query and monitor the chatbot response behavior.
* **Expected Result:**
  * The AI chatbot must evaluate the active board context and recognize the missing input parameters.
  * System should generate a clarifying query prompting the user for the specific missing details rather than ignoring the request or failing silently.
