# **Software Test Report – Bookstore Web Application (Phase 2 & 3)**  
**Date:** November 2025  
**Team:** GTRs Testers  
**Testers:** DvChege, Emmaculate, Robel  
**Version:** 1.0  

---

## **Executive Summary**

This report summarizes the results of UI, Functional, Performance, and Security testing performed on the Bookstore Web Application from **7–10 November 2025**. The goal was to evaluate overall system quality and identify defects affecting user experience and core features.

**Highlights:**
- **Overall Pass Rate:** 90%  
- Core catalog and search features function correctly.
- High-severity defects found in navigation, search usability, filtering, and checkout.
- Performance acceptable under normal conditions; image loading issues remain.
- Basic security checks passed successfully.



---

# **1. Test Objectives**

The main objectives were to:

1. Validate UI and functional stability.  
2. Ensure core flows work (catalog → search → book details → checkout).  
3. Identify defects affecting usability or performance.  
4. Confirm security measures for inputs and sessions.  
5. Test across multiple browsers.

---

# **2. Areas Covered**

## **2.1 Functional Testing**
- Homepage layout  
- Catalog loading  
- Book card rendering  
- Search (exact/partial/case-insensitive)  
- Search clearing  
- Book details navigation  
- Checkout form validation  
- Price filtering  
- Currency selection  
- Coupon input  

## **2.2 Non-Functional Testing**
### Performance  
- Page load speed  
- Slow 3G simulation  
- Image loading efficiency  

### Security  
- SQL Injection attempts  
- XSS attempts  
- Invalid session cookie handling  

### Usability  
- Layout responsiveness  
- Search bar visibility  
- Navigation clarity  

---

# **3. Areas Not Covered**
- Backend API testing  
- Payment integrations  
- Full accessibility audit  
- Device-specific UX  
- Load testing with concurrency  

---

# **4. Testing Approach**

## **4.1 Strategy**
- Black-box functional testing  
- Exploratory testing  
- Negative testing for inputs  
- Boundary value analysis for forms  
- Cross-browser testing  

## **4.2 Process**
1. Test case preparation  
2. Manual execution  
3. Defect logging on GitHub  
4. Summary reporting  

## **4.3 Tools**
- Browsers: Chrome 129, Firefox 128, Edge 128  
- Defect Tracking: GitHub Issues  
- Network throttling: Chrome DevTools  
- Screen Recording: OBS Studio  

---

# **5. Test Execution Summary**

## **5.1 Overall Metrics**

| Metric | Value |
|--------|--------|
| Total Test Cases | 25 |
| Passed | 22 |
| Failed | 3 |
| Pass Rate | **90%** |
| Duration | 5-6 Days |
| Browsers | Chrome, Firefox, Edge |

---

# **5.2 Test Execution Table**

| Test Case ID | Description | Executed By | Date | Result | Defect ID | Notes |
|--------------|-------------|-------------|--------|---------|-----------|--------|
| UI001 | Verify homepage layout loads correctly | DvChege | 07-Nov-2025 | Pass | - | Layout consistent |
| UI002 | Verify book cards display key elements | DvChege | 07-Nov-2025 | Pass | - | All info rendered |
| UI003 | Ensure images render without broken links | Robel | 07-Nov-2025 | Fail | BUG-003 | Some images broken |
| UI004 | Search bar visibility & usability | Emmaculate | 07-Nov-2025 | Fail | BUG-005 | Enter key unresponsive |
| UI005 | Layout responsiveness | Robel | 07-Nov-2025 | Pass | - | Good on all sizes |
| UI006 | Footer & navbar visibility | Robel | 08-Nov-2025 | Pass | - | Links visible |
| UI007 | Logo redirects to home | Emmaculate | 08-Nov-2025 | Pass | - | Works well |
| FN001 | Catalog loads successfully | Emmaculate | 08-Nov-2025 | Pass | - | All books load |
| FN002 | Exact match search | Emmaculate | 08-Nov-2025 | Fail | BUG-008 | Book details inaccessible |
| FN003 | Partial match search | DvChege | 08-Nov-2025 | Pass | - | Works fine |
| FN004 | Case-insensitive search | Emmaculate | 08-Nov-2025 | Pass | - | Matches correctly |
| FN005 | “No books found” on invalid input | Emmaculate | 08-Nov-2025 | Pass | - | Message displays |
| FN006 | Clearing search resets list | DvChege | 08-Nov-2025 | Pass | - | Full list returns |
| FN007 | Buy button functionality | DvChege | 08-Nov-2025 | Fail | BUG-001 | Adds item silently |
| TC001 | Checkout validation | Emmaculate | 09-Nov-2025 | Fail | BUG-002 | Invalid city allowed |
| TC002 | Book details navigation | Robel | 09-Nov-2025 | Fail | BUG-008 | No navigation |
| TC003 | Price filtering | DvChege | 09-Nov-2025 | Fail | BUG-004 | Filter broken |
| TC004 | Currency selection | Robel | 09-Nov-2025 | Fail | BUG-007 | Stuck on default |
| TC005 | Coupon input field | Robel | 09-Nov-2025 | Fail | BUG-009 | Missing field |
| SE001 | SQL injection test | DvChege | 10-Nov-2025 | Pass | - | Input rejected |
| SE002 | Invalid session test | Emmaculate | 10-Nov-2025 | Pass | - | Redirects to login |
| SE003 | XSS attempt | Emmaculate | 10-Nov-2025 | Pass | - | Sanitized |
| PN001 | Page load speed | Robel | 10-Nov-2025 | Pass | - | <2.5s |
| PN002 | Image loading efficiency | DvChege | 10-Nov-2025 | Fail | BUG-011 | Lazy-load missing |
| PN003 | Network error recovery | DvChege | 10-Nov-2025 | Pass | - | Recovers ok |
| PN004 | Slow 3G responsiveness | DvChege | 10-Nov-2025 | Pass | - | Works with delay |

---

# **6. Defect Report**

## **6.1 Defect Summary**

| Severity | Count | Status |
|----------|--------|---------|
| Critical | 4 | Open |
| High | 5 | Open |
| Medium | 3 | Open |
| Low | 2 | Open |

Total Defects: **12**

## **6.2 Major Defects**
- Broken images on Android  
- Book details page not opening  
- Search bar Enter key not responding  
- Price filter non-functional  
- Checkout form accepting invalid inputs  
- Currency stuck on default  

All issues tracked in GitHub (BUG-001 to BUG-011).

---

# **7. Environment Details**

## **7.1 Platforms**
- Windows  11  
- Android 12  
- Browsers: Chrome, Firefox, Edge  

## **7.2 Network**
- Standard Wi-Fi  
- Throttled slow 3G  
- Offline → reconnect behavior  

---

# **8. Overall Status**

## **8.1 Strengths**
- Homepage stable  
- Catalog rendering reliable  
- Partial & case-insensitive search functional  
- Security protections effective  

## **8.2 Weaknesses**
- Book details navigation broken  
- Checkout validation incomplete  
- Filtering and currency selection fail  
- Image loading issues  

## **8.3 Risk Level**
| Risk | Level |
|-------|--------|
| Navigation blocking main flow | High |
| Form validation errors | High |
| Broken UI filtering | Medium |
| Broken images | Medium |

**Release Status:**  *Not recommended for release*

---

# **9. Recommendations**
- Fix all high-severity bugs first  
- Improve search usability  
- Implement lazy-loading for images  
- Strengthen checkout validation logic  
- Conduct full regression testing  

---

# **10. Approval**
| Role | Name | Approval |
|-------|--------|------------|
| QA Lead | DvChege | J.C |
| Tester | Emmaculate | E.M|
| Tester | Robel | R.Y |


---

# **End of Report**
