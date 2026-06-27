# Requirements Traceability Matrix (RTM)

This RTM demonstrates clear traceability between Test Scenarios (TS), Test Cases (TC), and Bug Reports (BUG) for the AI-Powered Search Platform.

It shows that manual testing was conducted in a structured, requirement-driven manner, covering critical user journeys such as query handling, dynamic filter logic, and result formatting.

| Requirement ID | Requirement Description | Test Scenario | Test Case | Bug |
| :--- | :--- | :--- | :--- | :--- |
| ASP-REQ-001 | Search field accepts alphanumeric queries and special character criteria | TS-ASP-001 | TC-ASP-001 | Passed |
| ASP-REQ-002 | Filters dynamically update total product counts based on active query params | TS-ASP-002 | TC-ASP-002 | BUG-ASP-009 |
| ASP-REQ-003 | System renders a prominent 'No Results Found' view for invalid string inputs | TS-ASP-003 | TC-ASP-003 | Passed |
| ASP-REQ-004 | Search auto-suggest dropdown displays relevant keyword predictions instantly | TS-ASP-004 | TC-ASP-004 | BUG-ASP-015 |
| ASP-REQ-005 | Sorting parameters (Price, Relevance, Date) reorder data arrays correctly | TS-ASP-005 | TC-ASP-005 | Passed |
| ASP-REQ-006 | Search results page retains pagination state when navigating back from a link | TS-ASP-006 | TC-ASP-006 | BUG-ASP-002 |
| ASP-REQ-007 | High-volume query traffic does not cause layout shifts or skeleton breaks | TS-ASP-007 | TC-ASP-007 | Passed |
| ASP-REQ-008 | Recent search queries are securely stored and retrievable in user search history | TS-ASP-008 | TC-ASP-008 | Passed |

---

## Purpose
The RTM ensures that:
* Every business requirement is linked to a test scenario
* Each test scenario is validated through at least one test case
* All identified bugs are traceable to specific test executions
* Core search flows (query evaluation, facets, auto-suggestions) are fully tested
* QA coverage is transparent, auditable, and portfolio-ready

## Tools Used
* **Jira** – defect reporting and tracking
* **Chrome DevTools** – UI, layout, and responsive testing
* **Markdown** – documentation format
* **GitHub** – portfolio presentation

## NDA Notice
All identifiers, flows, and examples are anonymized. No real client data, URLs, or proprietary business logic are included. This RTM is shared only to demonstrate QA structure, methodology, and traceability.
