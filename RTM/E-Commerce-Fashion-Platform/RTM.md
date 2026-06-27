# Requirements Traceability Matrix (RTM)

This RTM demonstrates clear traceability between Test Scenarios (TS), Test Cases (TC), and Bug Reports (BUG) for the E-Commerce Fashion Platform.

It shows that manual testing was conducted in a structured, requirement-driven manner, covering critical user journeys such as discount logic rules, inventory configurations, and branch pickup dependencies.

| Requirement ID | Requirement Description | Test Scenario | Test Case | Bug |
| :--- | :--- | :--- | :--- | :--- |
| ECOM-REQ-001 | Expired/exhausted promo codes (count = 0) must be rejected during verification | TS-ECFP-005 | TC-ECFP-005 | BUG-ECFP-001 |
| ECOM-REQ-002 | 'In-Store Pickup' option must be hidden/disabled for 'Online Only' inventory items | TS-ECFP-001 | TC-ECFP-001 | BUG-ECFP-002 |
| ECOM-REQ-003 | Physical store pickup menus must dynamically list branches with available stock | TS-ECFP-002 | TC-ECFP-002 | BUG-ECFP-003 |
| ECOM-REQ-004 | Checkout submittal is blocked if mandatory shipping rows contain blank entries | TS-ECFP-004 | TC-ECFP-004 | Passed |
| ECOM-REQ-005 | Intercepted or modified negative values inside cart quantity arrays are rejected | TS-ECFP-003 | TC-ECFP-003 | BUG-ECFP-004 |
| ECOM-REQ-006 | Changing the region dropdown refreshes localized currency modifiers correctly | TS-ECFP-006 | TC-ECFP-006 | Passed |
| ECOM-REQ-007 | Payment interface handles boundary edge case values without breaking total sum | TS-ECFP-007 | TC-ECFP-007 | Passed |
| ECOM-REQ-008 | Cart total price automatically syncs when items are removed via line actions | TS-ECFP-008 | TC-ECFP-008 | Passed |

---

## Purpose
The RTM ensures that:
* Every business requirement is linked to a test scenario
* Each test scenario is validated through at least one test case
* All identified bugs are traceable to specific test executions
* Core transactional flows (checkout filters, pricing rules, cart limits) are fully tested
* QA coverage is transparent, auditable, and portfolio-ready

## Tools Used
* **Jira** – defect reporting and tracking
* **Chrome DevTools** – UI, layout, and responsive testing
* **Markdown** – documentation format
* **GitHub** – portfolio presentation

## NDA Notice
All identifiers, flows, and examples are anonymized. No real client data, URLs, or proprietary business logic are included. This RTM is shared only to demonstrate QA structure, methodology, and traceability.
