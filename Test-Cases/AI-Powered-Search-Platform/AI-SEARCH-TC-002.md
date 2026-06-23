## AI-SEARCH-TC-002 – Verify Dynamic Language Switching And Context Retention In AI Chat Widget

* **Related Bug:** AI-SEARCH-BUG-001, AI-SEARCH-BUG-003  
* **Module:** AI Chatbot Widget  
* **Type:** Localization / Integration Test  
* **Priority:** High  

### Precondition
* The global application layout is configured to English ("ENG") mode.
* The AI Chat Assistant panel is open and active.

### Steps
1. Submit an initial greeting query in English: "Hello, I need some assistance."
2. Change the chat interface language configuration to Georgian using the inline language selector dropdown.
3. Submit a specific product inquiry completely in English (e.g., "Show me the latest laptop models").
4. Observe the language model output generation and interface element behaviors.

### Expected Result
* The AI Assistant must dynamically adapt to the selected language state.
* Upon switching to Georgian, system messages, the input placeholder ("დაწერე შეტყობინება..."), and subsequent AI responses must render in Georgian.
* The initial welcome message should localize correctly and not remain hardcoded in English.
