# Bookstore App – QA Testing Presentation Script

**Team:** GTRs Testers  
**Presenter:** Emmaculate & Josphat
**Date:** November 2025 
**Duration:** 5 Minutes  

---

## 1. Introduction 

Hello, my name is Emmaculate from the GTRs Testing Team.  
My team Members include; Robel Yihelu(team lead), Josphat Chege(QA Analyst 7 planner) and Emmaculate Mumbua(test executor & documentation lead)
This presentation summarizes our QA testing for the Bookstore Application, covering UI, Functional, Performance, and Security testing.

**Scope included:**
- Homepage UI validation  
- Search feature behavior  
- Book details navigation  
- Checkout form validation  
- Cart operations  
- Performance and security tests  

## 2. Test Approach 

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

## 3. Key Findings 

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


### UI and Navigation Issues

#### BUG-005 — Center Search bar not functional (FR-O01)
Pressing Enter does not trigger search.

#### BUG-006 — Navigation links not clickable (FR-O02)
Only the logo works for navigation.

### Performance Issue

#### BUG-011 — Missing lazy-loading (FR-X02)
Images load all at once, slowing down the page.

## Test Execution & Evidence
We executed 25 test cases focusing on:
- Book Listing and Details  
- Cart operations  
- Checkout process  
Screenshots were captured to provide visual evidence of each module in action.  
For example, the **Cart Page** showed subtotal calculations, and the **Checkout Page** demonstrated input form validation.

  
## Summary & Analysis
Out of 25 test cases:
- **22 passed** successfully  
- **3 failed** initially but are under review  
Overall, the app achieved **90% test coverage**, showing reliable performance with a few areas for improvement.

## 4. Demo – Major Defect 

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


## 5. Recommendations 

### High Priority Fixes
- Fix book detail navigation  
- Make search bar responsive  
- Strengthen form validations  
- Add user feedback for cart actions   
- Make all navbar links functional  

### Additional Improvements
- Add automated regression tests  
- Add unit tests for search and filter logic  
- Improve caching for mobile devices  

## 6. Closing 

The Bookstore App is functional but requires improvements in navigation, search accuracy, validation, and UI responsiveness.  
This testing cycle enhanced the app's overall quality and aligned results with functional requirements.

Thank you for reviewing this presentation.
**GTRs Testers**

