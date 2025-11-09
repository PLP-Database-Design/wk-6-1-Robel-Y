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
| `screenshots/` | Screenshots of executed test results |

---

## 7. Testing Approach
| Type | Description |
|------|-------------|
| **Manual UI Testing** | Observe visual layout, spacing, and responsiveness |
| **Functional Testing** | Input search queries and verify outcome |
| **Regression Testing** | Re-run tests after any UI fixes |

No automation testing is included in this phase.

---
## 9. UI/UX Considerations
The testing in this phase also evaluates the usability and visual quality of the Bookstore Application.  
This includes:

- Clarity and readability of fonts and text
- Consistency of spacing and layout across devices
- Visibility and usability of the search bar
- Proper display of book cards (Image, Title, Author, Price)
- User experience when searching (results appear in real time)

A clean and simple UI is expected to help users navigate and find books efficiently.


## 8. Risks & Assumptions
| Risk | Impact | Mitigation |
|------|--------|------------|
| Search malfunction due to case sensitivity | Medium | Test using multiple input variations |
| Missing Book Details Page | High | Log defect and schedule feature for Phase 3 |
| No backend/database | Low | Local data allowed for offline testing |

---

## 9. Approval
| Name | Role | Signature | Date |
|------|------|-----------|------|
| DvChege | Tester | — | — |
| Robel | QA Lead | — | — |
| Immaculate | Documentation Lead | — | — |

---

**End of Test Plan**
