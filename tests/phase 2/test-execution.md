# Test Execution Report – Bookstore Application (Phase 2)

**Team:** GTRs Testers  
**Tester:** DvChege  
**Date:** November 2025  

This report documents the execution results of all UI and Functional test cases for the Bookstore Application, including Pass/Fail status, defects, and observations.

---

## 1. Test Execution Table

| Test Case ID | Description | Executed By | Date Executed | Result | Defect ID | Notes |
|--------------|-------------|--------------|----------------|----------|-------------|--------|
| UI001 | Verify homepage layout loads correctly | DvChege | 10/11/2025 | Pass | - | Homepage elements displayed correctly without distortion |
| UI002 | Verify book cards display image, title, author, price | DvChege | 10/11/2025 | Pass | - | All cards displayed expected content |
| UI003 | Ensure all book images render without broken links | DvChege | 10/11/2025 | Pass | - | No broken or missing images found |
| UI004 | Verify search bar visibility and usability | DvChege | 10/11/2025 | Pass | - | Search bar visible and responsive |
| UI005 | Check layout responsiveness on window resize | DvChege | 11/11/2025 | Pass | - | Layout adjusts seamlessly on mobile and desktop views |
| UI006 | Verify footer links are working correctly | DvChege | 11/11/2025 | Pass | - | Footer links redirect to expected pages |
| UI007 | Validate color contrast and font visibility | DvChege | 11/11/2025 | Pass | - | Colors meet accessibility standards |
| FN001 | Verify book catalog loads successfully | DvChege | 11/11/2025 | Pass | - | All books displayed within 2 seconds |
| FN002 | Validate search returns exact match results | DvChege | 11/11/2025 | Pass | - | Accurate results displayed for exact keyword |
| FN003 | Validate search returns partial match results | DvChege | 11/11/2025 | Pass | - | Partial keyword search returns relevant results |
| FN004 | Ensure search is case-insensitive | DvChege | 11/11/2025 | Pass | - | Search results consistent for upper/lowercase inputs |
| FN005 | Display “No books found” on invalid input | DvChege | 11/11/2025 | Pass | - | Proper message displayed for unmatched terms |
| FN006 | Clearing search returns full book list | DvChege | 11/11/2025 | Pass | - | Full catalog restored after clearing input |
| FN007 | Verify Buy button action (expected no function) | DvChege | 11/11/2025 | Fail | D002 | Buy button not functional; feature pending implementation |
| TC001 | Validate add-to-cart logic (placeholder) | DvChege | 12/11/2025 | Fail | D003 | Add-to-cart feature unresponsive |
| TC002 | Validate login button (expected inactive) | DvChege | 12/11/2025 | Fail | D004 | Login form not implemented |
| TC003 | Confirm consistent data rendering across pages | DvChege | 12/11/2025 | Pass | - | Data consistency maintained across navigation |
| TC004 | Validate error handling for empty search field | DvChege | 12/11/2025 | Pass | - | No crash; empty input handled correctly |
| TC005 | Verify reload maintains UI structure | DvChege | 12/11/2025 | Pass | - | Layout remains consistent after refresh |
| SE001 | Test HTML form input validation | DvChege | 12/11/2025 | Pass | - | Validation messages displayed correctly |
| SE002 | Test if developer tools expose sensitive data | DvChege | 12/11/2025 | Pass | - | No sensitive data found in console |
| SE003 | Verify input fields prevent script injection | DvChege | 12/11/2025 | Pass | - | Basic input sanitization confirmed |
| PN001 | Verify page load speed under normal conditions | DvChege | 12/11/2025 | Pass | - | Loads within acceptable 2–3 second range |
| PN002 | Verify response time for search function | DvChege | 12/11/2025 | Pass | - | Search executes under 1 second |
| PN003 | Verify app stability on repeated reload | DvChege | 12/11/2025 | Pass | - | Stable after multiple reloads |
| PN004 | Monitor performance with multiple open tabs | DvChege | 12/11/2025 | Pass | - | No crashes or lag noticed |

---

## 2. Execution Notes

- **Testing Method:** Manual execution using Google Chrome browser on desktop and Android devices.  
- **Defect Tracking:** All failing tests have been logged in the `defect-log.md` file with severity and priority levels.  
- **Evidence:** Screenshots captured for both passing and failing tests stored in `/screenshots/Phase3/`.  
- **Environment:** VS Code Live Server, Google Chrome v118, and local JSON data for book catalog.  
- **Traceability:** Each test case corresponds to requirements defined in the Test Plan (Phase 1).  

---

 **Summary:**  
- **Total Test Cases Executed:** 25  
- **Passed:** 22  
- **Failed:** 3  
- **Overall Pass Rate:** 90%  
- **Application Status:** Functionally stable; pending implementation of Buy and Login features.  

---

**End of Test Execution Report**
