## AI-CONTENT-TC-005 – Verify Category Dropdown Link Routing Logic Within Global Header

* **Related Bug:** AI-CONTENT-BUG-005  
* **Module:** Header Navigation Routing  
* **Type:** Integration / Functional Test  
* **Priority:** High  

### Precondition
* The user is on the main application interface.

### Steps
1. Interact with the "News" category dropdown module inside the primary navigation header layout.
2. Click directly on the designated "News/Blog" subcategory option link.
3. Observe the newly loaded page layout, structural view components, and browser URL destination path.

### Expected Result
* The system routing mechanism must resolve the action to the correct target endpoint destination.
* The browser must load the dedicated, relevant news content timeline layout.
* The action must not incorrectly redirect the user to unrelated grid items (such as "Games/Projects").
