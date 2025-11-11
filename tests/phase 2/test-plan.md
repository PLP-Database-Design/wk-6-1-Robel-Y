# Test Plan – Bookstore Application (Phase 2)
**Team:** GTRs Testers  
**Project:** Bookstore App  
**Tester:** DvChege  
**Date:** November 2025  

---

## 1. Introduction
This Test Plan outlines the testing approach for the Bookstore Application during Phase 2.  
The main goal is to verify the User Interface (UI) and Search functionality based on the current system implementation, where book data is stored locally in a JavaScript array.

---

## 2. Scope of Testing

### **In-Scope**
The following features will be tested:
- Display of Book Catalog
- Search Function Functionality
- UI Layout & Responsiveness
- “Buy Now” Button Presence (No functionality expected)

### **Out-of-Scope (To be implemented in Phase 3)**
The following features are *not* currently implemented and therefore will not be tested:
- User Login / Authentication
- Admin Dashboard
- Shopping Cart and Checkout Process
- Book Details Page Navigation

---

## 3. Test Objectives
- Ensure that the book catalog loads correctly.
- Verify that the search bar filters books correctly based on input.
- Confirm that the UI layout is clear, readable, and responsive.
- Document defects and missing functionalities for improvement in Phase 3.

---

## 4. Test Environment
| Component | Description |
|----------|-------------|
| Device | Laptop / Desktop |
| Browser | Chrome / Firefox / Edge |
| Data Source | Local JavaScript array of books |
| Network | Not required (No server calls) |

---

## 5. Test Items
- Homepage / Book Catalog Page
- Search Bar Component
- Book Display Cards
- Buy Button (non-functional verification)

---

## 6. Test Deliverables
| Deliverable | Description |
|------------|-------------|
| `test-cases.md` | UI and Functional test cases |
| `test-execution.md` | Execution results (Pass / Fail) |
| `defect-log.md` | List of defects found during testing |
| `screenshots/` | Evidence of executed test results |

---

## 7. Testing Approach
| Type | Description |
|------|-------------|
| **Manual UI Testing** | Observe visual layout, spacing, and responsiveness |
| **Functional Testing** | Input search queries and verify outcome |
| **Regression Testing** | Re-run tests after any UI fixes |

No automation testing is included in this phase.

---

## 8. Risks & Assumptions
| Risk | Impact | Mitigation |
|------|--------|------------|
| Search malfunction due to case sensitivity | Medium | Test using multiple input variations |
| Missing Book Details Page | High | Log defect and schedule feature for Phase 3 |
| No backend/database | Low | Local data allowed for offline testing |

---

## 9. UI/UX Considerations
UI/UX Testing focuses on usability and visual quality:

- Consistency of font sizes and spacing
- Clear and readable text
- Image and card alignment
- Search bar usability and visibility
- Responsiveness across devices

A clean UI helps support easier user navigation and book discovery.

---

## 10. Team Contribution Statement – Phase 2

During Phase 2, the team collaborated on test planning, UI evaluation, test documentation, and defect tracking.

| Team Member | Responsibilities Completed |
|------------|----------------------------|
| **Emma** | - Created and assigned team roles  
- Reviewed the Test Plan and Test Cases  
- Created and maintained the Defect Log  
- Logged and updated identified defects in GitHub |
| **Bashir** | - Designed and documented the Test Cases  
- Created the UI/UX Functional Design Checklist  
- Structured and organized Test Execution approach  
- Assisted in defect tracking and documentation |

### Team Scoring

| Team Member | Contribution Quality (1–10) | Participation (1–10) | Reliability (1–10) | **Final Score (Avg)** |
|------------|-----------------------------|----------------------|--------------------|----------------------|
| **Emma** | 9 | 8 | 9 | **8.7** |
| **Bashir** | 10 | 9 | 10 | **9.7** |
| **Robel** |4 | 2 | 2 |**5.5**|

> Both members contributed effectively. Emma led coordination and defect management; Bashir led documentation and UI/functional structuring.

---

## 11. Approval
| Name | Role | Signature | Date |
|------|------|-----------|------|
| DvChege | Tester | — | — |
| Robel | QA Lead | — | — |
| Immaculate | Documentation Lead | — | — |

---

**End of Test Plan**
