# Bookstore App – QA Testing Presentation (Phase 2 & 3)

**Team:** GTRs Testers  
**Presenter:** Emmaculate  
**Date:** November 2025  

---

## 1. Introduction (30s)

Hello, my name is Emmaculate from the GTRs Testing Team.  
This presentation summarizes our QA testing for the Bookstore Application, covering UI, Functional, Performance, and Security testing.

**Scope included:**
- Homepage UI validation  
- Search feature behavior  
- Book details navigation  
- Checkout form validation  
- Cart operations  
- Performance and security tests  

## 2. Test Approach (60s)

### Tools Used
- Browsers: Chrome 129, Firefox 128, Edge 128  
- Devices: Windows 10/11, macOS 14, Android 12  
- Tools: VS Code, Jira, Chrome DevTools and Github
- Evidence stored in `/screenshots/` folder

### Testing Strategy
- Manual execution of predefined test cases  
- Exploratory testing for navigation and field validation  
- Negative tests: invalid inputs  
- Performance tests: load time, lazy-loading, slow network  

### Data Strategy
- Realistic book titles and price values  
- Valid and invalid text inputs  
- Edge cases: symbols, long strings, case variations  

## 3. Key Findings (120s)

A total of 14 defects were logged:
- 8 Major/Critical  
- 6 Medium/Minor  

### Critical Functional Issues

#### BUG-001 — "Buy Now" adds items silently (FR-O01)
**Expected:** Confirmation or cart badge increment  
**Actual:** User receives no feedback  

#### BUG-002 — Invalid city accepted (FR-O02)
Form validation accepts incorrect city input.

#### BUG-004 — Price filter not working (FR-O01)
Filter does not update product list.

#### BUG-008 — Cannot open book details (FR-O04)
Book card click does nothing.


### UI and Navigation Issues

#### BUG-005 — Search bar not functional (FR-O01)
Pressing Enter does not trigger search.

#### BUG-006 — Navigation links not clickable (FR-O02)
Only the logo works for navigation.



### Performance Issue

#### BUG-011 — Missing lazy-loading (FR-X02)
Images load all at once, slowing down the page.

---

### User Impact Summary
- Core user journey interruptions  
- Navigation limitations  
- Weak input validation  
- Slower mobile performance  

---

## 4. Demo – Major Defect (60s)

### BUG-008 — Book Details Page Not Opening

**Steps:**
1. Open the catalog  
2. Click on any book  

**Expected:**  
Book details page displays title, author, price, and description.

**Actual:**  
Nothing happens; click event is not triggered.

**Impact:**  
Users cannot view product details before purchasing. This blocks the main buying flow.

---

## 5. Recommendations (30s)

### High Priority Fixes
- Fix book detail navigation  
- Make search bar responsive  
- Strengthen form validations  
- Add user feedback for cart actions  
- Implement lazy-loading for performance  
- Make all navbar links functional  

### Additional Improvements
- Add automated regression tests  
- Add unit tests for search and filter logic  
- Improve caching for mobile devices  

---

## 6. Closing (20s)

The Bookstore App is functional but requires improvements in navigation, search accuracy, validation, and UI responsiveness.  
This testing cycle enhanced the app's overall quality and aligned results with functional requirements.

Thank you for reviewing this presentation.



# Phase 3 – Video Presentation Script  
**Team:** GTRs Testers  
**Application:** Bookstore App  
**Presenter:** DvChege  
**Duration:** 5 Minutes  

---

## 🎤 Presentation Outline

### 1. Introduction
Hello everyone, my name is **DvChege**, representing the **GTRs Testers** team.  
This video covers **Phase 3 of our Bookstore Application testing**, where we performed final test execution, defect reporting, and a comprehensive summary of results.

---

### 2. Testing Objective
Our main objective was to verify the end-to-end functionality of the Bookstore App — from browsing books, adding to cart, to completing checkout — ensuring that all workflows operate as expected and meet user requirements.

---

### 3. Test Execution & Evidence
We executed 25 test cases focusing on:
- Book Listing and Details  
- Cart operations  
- Checkout process  
Screenshots were captured to provide visual evidence of each module in action.  
For example, the **Cart Page** showed subtotal calculations, and the **Checkout Page** demonstrated input form validation.

---

### 4. Defect Reporting
We recorded 3 key defects:
- Missing validation on required fields (High severity)  
- Subtotal delay after removing items (Medium severity)  
- Quantity field accepting letters (Low severity, later resolved)

Each issue was prioritized, reported, and assigned to the respective developer for resolution.

---

### 5. Summary & Analysis
Out of 25 test cases:
- **22 passed** successfully  
- **3 failed** initially but are under review  
Overall, the app achieved **90% test coverage**, showing reliable performance with a few areas for improvement.

---

### 6. Conclusion
The Bookstore Application is functionally stable and ready for user acceptance testing after minor fixes.  
We recommend automating future regression tests and improving form validations.  

Thank you for watching our Phase 3 presentation.  
**– GTRs Testers**

