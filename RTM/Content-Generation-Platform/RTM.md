# Requirements Traceability Matrix (RTM)

This RTM demonstrates clear traceability between Test Scenarios (TS), Test Cases (TC), and Bug Reports (BUG) for the Content Generation Platform.

It shows that manual testing was conducted in a structured, requirement-driven manner, covering critical user journeys such as multimedia handling, story node navigation, and container alignment.

| Requirement ID | Requirement Description | Test Scenario | Test Case | Bug |
| :--- | :--- | :--- | :--- | :--- |
| CGP-REQ-001 | Media containers dynamically scale and align across responsive breakpoints | TS-CGP-001 | TC-CGP-001 | Passed |
| CGP-REQ-002 | System fallback renders an asset placeholder if multimedia components fail to load | TS-CGP-002 | TC-CGP-002 | BUG-CGP-004 |
| CGP-REQ-003 | End-to-end user navigation funnels prevent logical dead-ends during creation | TS-CGP-003 | TC-CGP-003 | Passed |
| CGP-REQ-004 | Export module renders final generated text files cleanly without script tags | TS-CGP-004 | TC-CGP-004 | BUG-CGP-011 |
| CGP-REQ-005 | Draft auto-save mechanism triggers successfully every 30 seconds of activity | TS-CGP-005 | TC-CGP-005 | Passed |
| CGP-REQ-006 | Animated interactive canvases execute without performance or frame drops | TS-CGP-006 | TC-CGP-006 | BUG-CGP-007 |
| CGP-REQ-007 | Localized interface fonts render consistently across default browser matrices | TS-CGP-007 | TC-CGP-007 | Passed |
| CGP-REQ-008 | Character profile images preserve correct aspect ratios on grid views | TS-CGP-008 | TC-CGP-008 | Passed |

---

## Purpose
The RTM ensures that:
* Every business requirement is linked to a test scenario
* Each test scenario is validated through at least one test case
* All identified bugs are traceable to specific test executions
* Core storytelling flows (canvas layout, media parsing, template generation) are fully tested
* QA coverage is transparent, auditable, and portfolio-ready

## Tools Used
* **Jira** – defect reporting and tracking
* **Chrome DevTools** – UI, layout, and responsive testing
* **BrowserStack** – cross-browser fidelity checking
* **Markdown** – documentation format
* **GitHub** – portfolio presentation

## NDA Notice
All identifiers, flows, and examples are anonymized. No real client data, URLs, or proprietary business logic are included. This RTM is shared only to demonstrate QA structure, methodology, and traceability.
