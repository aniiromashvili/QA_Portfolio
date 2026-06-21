## AI-CONTENT-TC-002 – Verify Mandatory Input Field Validation Constraints On Content Forms

* **Related Bug:** AI-CONTENT-BUG-002  
* **Module:** Form Validation Engine  
* **Type:** Boundary / Functional Test  
* **Priority:** Critical  

### Precondition
* The user is positioned at the contact/feedback form section.

### Steps
1. Clear any pre-filled or cached data from the input forms.
2. Leave all mandatory text boxes, contact selection fields, and dropdowns completely blank.
3. Click the form submission button.
4. Inspect the client-side interface for error logs, error boundaries, and network traffic status.

### Expected Result
* The client-side form handler must block the submission attempt.
* Blank or invalid request payloads must not be transmitted to the environment server.
* Relevant input fields must highlight with error borders, and explicit inline validation messages (e.g., "This field is required") must render clearly.
