## AI-SEARCH-TC-003 – Verify Boundary Value Validation On AI Chat Input Payload

* **Related Bug:** AI-SEARCH-BUG-002  
* **Module:** AI Chatbot Input Validation  
* **Type:** Boundary / Robustness Test  
* **Priority:** High  

### Precondition
* The user is on the main application interface with the AI Chat widget initialized.

### Steps
1. Copy a large block of text characters exceeding the maximum allowable system constraint (e.g., a 3,000-character payload).
2. Paste the oversized string into the chat text input field.
3. Observe if any client-side character constraint metrics or validation warnings trigger.
4. Execute the transmission command by clicking the send icon.
5. Attempt to send a subsequent valid brief string (e.g., "Hi") immediately afterward.

### Expected Result
* Client-side interface should block the transmission of the oversized payload and display an explicit error indicator.
* The system must not enter an infinite "Processing" state.
* Subsequent valid requests must process normally and receive a server response without being blocked by prior pending states.
