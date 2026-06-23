## AI-SEARCH-TC-004 – Verify Search Relevance Parsing For Truncated Brand Synonyms And Hardware Generations

* **Related Bug:** AI-SEARCH-BUG-004  
* **Module:** Search Relevance Algorithm  
* **Type:** Algorithmic Relevance Test  
* **Priority:** High  

### Precondition
* The user is positioned at the core AI-powered search interface.

### Steps
1. Input a specific combined query consisting of a truncated brand token and a generational integer value: "app 16"
2. Execute the search query.
3. Evaluate the catalog taxonomy weights and sorting order of the initial returned assets.

### Expected Result
* Search relevance algorithm must prioritize hardware brand synonym mappings over minor features.
* The system should map the token to the correct consumer electronics brand, displaying premium hardware matching that generation at the top of the search grid.
* Unrelated appliances that contain "app control" features should not override core brand keywords.
