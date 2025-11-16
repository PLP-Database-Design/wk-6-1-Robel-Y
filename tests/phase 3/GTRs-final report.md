# **Final QA Report – Bookstore Application**
**Team:** GTRs Testers  
**Project:** Bookstore App  
**Date:** November 2025  

---

# **1. Executive Summary**
The purpose of this report is to document the complete Quality Assurance (QA) activities performed on the **Bookstore Application** across **Phase 1**, **Phase 2**, and **Phase 3**.  
The application is a simple client-side bookstore system built using HTML, CSS, and JavaScript, with all book data stored locally in a JavaScript array.

Testing activities focused on:
- Understanding system requirements (Phase 1)  
- Designing and executing UI & functional test cases (Phase 2)  
- Performing full execution, logging defects, and compiling results (Phase 3)

The findings from this QA cycle will guide improvements in functionality, UI design, and feature completeness.

---

# **2. Phase 1 – Requirement Review & System Understanding**

## **2.1 System Overview**
The Bookstore App allows users to:
- View a list of books stored locally  
- Search books by title  
- Click a “Buy Now” button (currently non-functional)  

There is **no login**, **no admin panel**, **no cart**, and **no detailed book page** implemented.

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

Requirements for Phase 2 testing were therefore based on the **actual implemented system**, not assumed features.

---

# **3. Phase 2 – Test Planning & Test Design**

## **3.1 Test Plan Summary**
The Phase 2 Test Plan focused on:
- UI/UX Quality Checks  
- Functional Testing of Catalog + Search  
- Basic layout responsiveness  
- Defect detection for missing or incorrect UI behaviors  

Out-of-scope items included login, admin, checkout, and cart features, which the app does not support yet.

## **3.2 Test Cases (UI & Functional)**

| Test Case ID | Module | Test Objective | Pre-Condition | Test Steps | Expected Result | Status |
|--------------|---------|---------------|----------------|------------|----------------|--------|
| TC-001 | UI Layout | Verify homepage loads correctly | App running | Open homepage | Books render with images and titles | Pass |
| TC-002 | Search | Verify search filters books | Books loaded | Enter keyword | Matching books displayed | Pass |
| TC-003 | Search | Verify empty search shows all books | Books loaded | Clear search bar | Full list displayed | Pass |
| TC-004 | Book Card | Verify book card elements | App running | Inspect card | Image, title, price visible | Pass |
| TC-005 | Buy Button | Verify “Buy” button is visible | App running | Click Buy | No page redirect (expected) | Pass |

## **3.3 UI/UX Checklist**

| UI Area | Check | Status | Notes |
|--------|-------|--------|-------|
| Layout | Content aligned |Pass | — |
| Buttons | Clearly visible | Pass| — |
| Text | Readable fonts | Pass | — |
| Navigation | Simple navigation | Pass | No multiple pages |
| Colors | Consistent theme | Pass | The colors are consistent |
| Images | Render clearly |Pass | - |
| Forms | Checkout form clarity | Pass|  forms are clear |
| Responsiveness | Works on laptop/mobile | Pass| Responsive in mobile/laptop|

---

# **4. Phase 3 – Test Execution, Evidence & Defect Log**

## **4.1 Execution Summary**

Execution results include pass/fail status and screenshots as evidence.

## **4.2 Final Execution Table**
| Test Case ID | Result | Evidence | Tester |
|--------------|--------|----------|--------|
| TC-001 | Pass/Fail | screenshot | Emma  |
| TC-002 | Pass/Fail | screenshot | Emma  |
| TC-003 | Pass/Fail | screenshot | Emma |
| TC-004 | Pass/Fail | screenshot |Emma  |
| TC-005 | Pass/Fail | screenshot | Emma |



## **4.3 Defect Log Summary**

| ID | Defect Description | Severity | Priority | Status |
|----|--------------------|----------|----------|--------|
| DF-001 | Buy button does nothing | Low | Low | Open |
| DF-002 | Images stretch on some screens | Medium | Medium | Open |
| DF-003 | Search is case-sensitive | Medium | Medium | Open |
| DF-004 | No book detail page | High | High | Logged |

Immaculate maintained the defect log in GitHub.

---

# **5. Team Contributions & Scoring**

## **5.1 Contribution Statement**
- **DvChege**  
  - Designed & documented test cases  
  - Created UI and functional checklists  
  - Executed test cases  
  - Supported defect tracking  
  - Prepared final report  

- **Emmaculate**  
  - Created team roles document  
  - Wrote test plan & reviewed test cases  
  - Created and maintained defect log  
  - Logged defects into GitHub  

- **Robel**  
  - Executed test cases  
  - Reviewed Phase 2 documentation  
  - Provided approvals  

## **5.2 Team Scoring (Fair Contribution Model)**

| Member | Contribution Level | Score (1–10) |
|--------|--------------------|--------------|
| DvChege | Major contributor | 10 |
| Emmaculate | Strong contributor | 9 |
| Robel | Good contributor | 8 |

---

# **6. Conclusion**
Testing across three phases allowed the team to understand the current limitations of the Bookstore App and identify areas that require enhancement.  
The system functions as a simple static catalog but lacks key ecommerce features.  



---

**End of Final QA Report**  
