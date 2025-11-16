# **Final QA Report – Bookstore Application**
**Team:** GTRs Testers  
**Project:** Bookstore App  
**Date:** November 2025  

---

# **1. Executive Summary**
This report documents the complete Quality Assurance (QA) activities performed on the **Bookstore Application** across **Phase 1**, **Phase 2**, and **Phase 3**.  

The application is a simple client-side bookstore system built using HTML, CSS, and JavaScript, with all book data stored locally in a JavaScript array.

Testing activities focused on:
- Understanding system requirements (Phase 1)  
- Designing and executing UI & functional test cases (Phase 2)  
- Performing full execution, logging defects, and compiling results (Phase 3)

Findings from this QA cycle will guide improvements in functionality, UI design, and feature completeness.

---

# **2. Phase 1 – Requirement Review & System Understanding**

## **2.1 System Overview**
The Bookstore App allows users to:
- View a list of books stored locally  
- Search books by title  
- Click a “Buy Now” button (currently non-functional)  

**Not Implemented in Phase 1:**
- Login / Admin panel  
- Cart  
- Book details page  

## **2.2 UI Screens Observed**
- Home / Book Catalog Page  
- Search Bar Section  
- Book Cards (Image, Title, Price)  
- Buy Button (inactive)

## **2.3 Functional Understanding**
| Feature | Status |
|--------|--------|
| Book Catalog Display | Implemented |
| Search Function | Implemented |
| Book Details Page | Not Implemented |
| Cart & Checkout | Not Implemented |
| Payments | Not Implemented |

Requirements for Phase 2 testing were based on **actual implemented features**.

---

# **3. Phase 2 – Test Planning & Test Design**

## **3.1 Test Environment & Platform Details**
| Platform | Version | Notes |
|---------|---------|-------|
| Windows 10 / 11 | Chrome 142, Edge 128 | Primary testing environment |
| macOS 14 | Firefox 128 | Cross-browser validation |
| Android 13 | Chrome Mobile | Mobile UI checks |
| iOS 26 | Safari Mobile | Responsiveness & touch testing |

## **3.2 Testing Tools Used**
| Tool | Purpose |
|------|---------|
| **Jira** | Test management, bug tracking, sprint organization |
| **GitHub** | Version control, repository collaboration, issue tracking |
| **Zoom** | Team communication, sprint reviews, defect triaging |
| **Chrome DevTools** | UI inspection, debugging, performance metrics |
| **VS Code** | Test development, notes, and documentation |

## **3.3 Test Plan Summary**
- UI/UX Quality Checks  
- Functional Testing of Catalog + Search  
- Layout responsiveness  
- Defect detection for missing/incorrect UI behaviors  

**Out-of-scope:** login, admin, checkout, and cart features.

## **3.4 Test Cases (UI & Functional)**

| Test Case ID | Module | Test Objective | Pre-Condition | Test Steps | Expected Result | Status |
|--------------|---------|---------------|----------------|------------|----------------|--------|
| TC-001 | UI Layout | Verify homepage loads correctly | App running | Open homepage | Books render with images and titles | Pass |
| TC-002 | Search | Verify search filters books | Books loaded | Enter keyword | Matching books displayed | Pass |
| TC-003 | Search | Verify empty search shows all books | Books loaded | Clear search bar | Full list displayed | Pass |
| TC-004 | Book Card | Verify book card elements | App running | Inspect card | Image, title, price visible | Pass |
| TC-005 | Buy Button | Verify “Buy” button is visible | App running | Click Buy | No page redirect (expected) | Pass |

## **3.5 UI/UX Checklist**

| UI Area | Check | Status | Notes |
|--------|-------|--------|-------|
| Layout | Content aligned | Pass | — |
| Buttons | Clearly visible | Pass | — |
| Text | Readable fonts | Pass | — |
| Navigation | Simple navigation | Pass | No multiple pages |
| Colors | Consistent theme | Pass | Colors consistent |
| Images | Render clearly | Pass | — |
| Forms | Checkout form clarity | Pass | Forms are clear |
| Responsiveness | Works on laptop/mobile | Pass | Responsive in mobile/laptop |

---

# **4. Phase 3 – Test Execution, Evidence & Defect Log**

## **4.1 Execution Summary**
Execution results include pass/fail status and screenshots/video evidence.

## **4.2 Final Execution Table**
| Test Case ID | Result | Evidence | Tester |
|--------------|--------|----------|--------|
| TC-001 | Pass | screenshot | Emma  |
| TC-002 | Pass | screenshot | Emma  |
| TC-003 | Pass | screenshot | Emma |
| TC-004 | Pass | screenshot | Emma  |
| TC-005 | Pass | screenshot | Emma |

## **4.3 Defect Log Summary**
| ID | Defect Description | Severity | Priority | Status |
|----|--------------------|----------|----------|--------|
| DF-001 | Buy button does nothing | Low | Low | Open |
| DF-002 | Images stretch on some screens | Medium | Medium | Open |
| DF-003 | Search is case-sensitive | Medium | Medium | Open |
| DF-004 | No book detail page | High | High | Logged |

**Note:** All defects are logged and maintained in GitHub by Emmaculate

## **4.4 Traceability Matrix**
| FR Code | Description | Related Test Cases | Defects Linked | Status |
|---------|-------------|------------------|----------------|--------|
| FR-O01 | Cart operations — add/remove/update with stock enforcement | TC-005, FN001, FN003 | DF-001 | Partial Failures |
| FR-O02 | Checkout wizard / validation | TC001, TC002 | DF-004 | Fail |
| FR-O03 | Payments — currency, Paystack init | N/A | None | Not Tested |
| FR-O04 | Catalog / Book detail | TC004, FN002 | DF-002, DF-003 | Partial Failures |
| FR-R01 | Returns — 7-day validation | N/A | None | Not Tested |
| FR-N02 | Notifications — mark all read | N/A | None | Not Tested |

**Summary:**  
- All FRs are linked to test cases and defects where applicable.  
- Critical defects are prioritized for remediation.

---

# **5. Team Contributions & Scoring**

## **5.1 Contribution Statement**
- **DvChege**: Designed & documented test cases, executed tests, supported defect tracking, prepared report.  
- **Emmaculate**: Created roles document, test plan, maintained defect log, logged defects into GitHub,, reviewed report.  
- **Robel**: Executed tests, reviewed documentation, provided approvals.

## **5.2 Approvals & Sign-Off**
| Name | Role | Status | Signature |
|------|------|--------|-----------|
| DvChege | QA Lead | Approved | J.C |
| Emma M | QA Tester | Approved | E.M |

---

# **6. Appendix**
Supporting materials included in `/screenshots/` and `/docs/` folders:
- Test cases  
- Defect logs  
- Traceability matrix  
- Environment and setup notes  

---

# **7. Conclusion**
Testing across three phases allowed the team to:
- Understand current limitations of the Bookstore App  
- Identify areas for improvement  
- Highlight missing ecommerce functionality (cart, checkout, payments, book detail)  

The system functions as a simple static catalog but requires enhancements for a complete user experience.

**End of Final QA Report**  
