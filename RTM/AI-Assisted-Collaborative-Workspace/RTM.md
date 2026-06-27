# Requirements Traceability Matrix (RTM)

This RTM demonstrates clear traceability between Test Scenarios (TS), Test Cases (TC), and Bug Reports (BUG) for the AI-Assisted Collaborative Workspace.

It shows that manual testing was conducted in a structured, requirement-driven manner, covering critical user journeys such as nested folder hierarchies, asset movement logic, and collaborative editor constraints.

| Requirement ID | Requirement Description | Test Scenario | Test Case | Bug |
| :--- | :--- | :--- | :--- | :--- |
| ACW-REQ-001 | System must support nested folder creation up to 5 levels deep | TS-ACW-001 | TC-ACW-001 | Passed |
| ACW-REQ-002 | Users can move assets between directories via drag-and-drop mechanics | TS-ACW-002 | TC-ACW-002 | BUG-ACW-004 |
| ACW-REQ-003 | Collaborative editor must enforce a 10,000 character limit per text block | TS-ACW-003 | TC-ACW-003 | BUG-ACW-012 |
| ACW-REQ-004 | System must prevent duplicate folder naming within the same directory level | TS-ACW-004 | TC-ACW-004 | Passed |
| ACW-REQ-005 | Editor changes must sync in real-time across active collaborative sessions | TS-ACW-005 | TC-ACW-005 | BUG-ACW-008 |
| ACW-REQ-006 | Rich text formatting controls (Bold, Italic, Lists) render consistently | TS-ACW-006 | TC-ACW-006 | Passed |
| ACW-REQ-007 | Workspace navigation and folder trees must be responsive on mobile screens | TS-ACW-007 | TC-ACW-007 | BUG-ACW-003 |
| ACW-REQ-008 | System gracefully handles character encoding and special symbols in file titles | TS-ACW-008 | TC-ACW-008 | Passed |

---

## Purpose
The RTM ensures that:
* Every business requirement is linked to a test scenario
* Each test scenario is validated through at least one test case
* All identified bugs are traceable to specific test executions
* Core workspace flows (file system, real-time sync, rich text editing) are fully tested
* QA coverage is transparent, auditable, and portfolio-ready

## Tools Used
* **Jira** – defect reporting and tracking
* **Chrome DevTools** – UI, layout, and responsive testing
* **Markdown** – documentation format
* **GitHub** – portfolio presentation

## NDA Notice
All identifiers, flows, and examples are anonymized. No real client data, URLs, or proprietary business logic are included. This RTM is shared only to demonstrate QA structure, methodology, and traceability.
