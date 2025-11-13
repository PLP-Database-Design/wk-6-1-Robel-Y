# Test Execution Report – Bookstore Application (Phase 2 & 3)

**Team:** GTRs Testers  
**Tester(s):** DvChege, Emmaculate, Robel
**Date:** November 2025  

This report documents the execution results of all UI and Functional test cases for the Bookstore Application, including Pass/Fail status, defects, and observations.

---

## 1. Test Execution Table

| Test Case ID | Description | Executed By | Date Executed | Result | Defect ID | Notes |
|--------------|--------------|--------------|----------------|----------|------------|--------|
| UI001 | Verify homepage layout loads correctly | DvChege | 07-Nov-2025 | Pass | - | Layout consistent with design |
| UI002 | Verify book cards display image, title, author, price | DvChege | 07-Nov-2025 | Pass | - | All book cards rendered correctly |
| UI003 | Ensure all book images render without broken links | Robel | 07-Nov-2025 | Fail | [BUG-003](https://github.com/PLP-Database-Design/wk-6-1-Robel-Y/issues/3#issue-3605378154) | Some images fail to load on Android |
| UI004 | Verify search bar visibility and usability | Emmaculate| 07-Nov-2025 | Fail | [BUG-005](https://github.com/PLP-Database-Design/wk-6-1-Robel-Y/issues/5#issue-3620175835) | Search bar not responsive on Enter |
| UI005 | Check layout responsiveness on window resize | Robel | 07-Nov-2025 | Pass | - | Works well on multiple resolutions |
| UI006 | Verify footer and navigation bar visibility | Robel | 08-Nov-2025 | Pass | - | Navigation visible; links limited |
| UI007 | Verify logo click redirects to home | Emmaculate | 08-Nov-2025 | Pass | - | Works as expected |
| FN001 | Verify book catalog loads successfully | Emmaculate | 08-Nov-2025 | Pass | - | Catalog loads with all listed books |
| FN002 | Validate search returns exact match results | Emmaculate | 08-Nov-2025 | Fail | [BUG-008](https://github.com/PLP-Database-Design/wk-6-1-Robel-Y/issues/8#issue-3620353811) | Cannot view book details |
| FN003 | Validate search returns partial match results | DvChege| 08-Nov-2025 | Pass | - | Works for partial words |
| FN004 | Ensure search is case-insensitive | Emmaculate | 08-Nov-2025 | Pass | - | "Harry" = "harry" |
| FN005 | Display “No books found” on invalid input | Emmaculate| 08-Nov-2025 | Pass | - | “No books found” message displays |
| FN006 | Clearing search returns full book list | DvChege | 08-Nov-2025 | Pass | - | Full list restored after clear |
| FN007 | Verify Buy button action (expected no function) | DvChege | 08-Nov-2025 | Fail | [BUG-001](https://github.com/PLP-Database-Design/wk-6-1-Robel-Y/issues/1#issue-3605368672) | Buy button adds item silently |
| TC001 | Validate checkout input form | Emmaculate | 09-Nov-2025 | Fail | [BUG-002](https://github.com/PLP-Database-Design/wk-6-1-Robel-Y/issues/2#issue-3605374428) | Invalid city accepted |
| TC002 | Validate book details page navigation | Robel | 09-Nov-2025 | Fail |[BUG-008](https://github.com/PLP-Database-Design/wk-6-1-Robel-Y/issues/8#issue-3620353811)  | Clicking book card does nothing |
| TC003 | Test price filtering | DvChege | 09-Nov-2025 | Fail | [BUG-004](https://github.com/PLP-Database-Design/wk-6-1-Robel-Y/issues/4#issue-3620153747) | Filter not working |
| TC004 | Test currency selection | Robel | 09-Nov-2025 | Fail | [BUG-007](https://github.com/PLP-Database-Design/wk-6-1-Robel-Y/issues/7#issue-3620333994) | Currency stuck on default |
| TC005 | Validate coupon input | Robel | 09-Nov-2025 | Fail | [BUG-009](https://github.com/PLP-Database-Design/wk-6-1-Robel-Y/issues/9#issue-3620370643) | No coupon field displayed |
| SE001 | SQL injection attempt on search field | DvChege | 10-Nov-2025 | Pass | - | System rejects malicious input |
| SE002 | Invalid session cookie test | Emmaculate | 10-Nov-2025 | Pass | - | App redirects to login |
| SE003 | Test XSS in search input | Emmaculate | 10-Nov-2025 | Pass | - | Input sanitized properly |
| PN001 | Page load time test (Chrome) | Robel | 10-Nov-2025 | Pass | - | Loads < 2.5s average |
| PN002 | Image loading efficiency | DvChege | 10-Nov-2025 | Fail | [BUG-011](https://github.com/PLP-Database-Design/wk-6-1-Robel-Y/issues/10#issue-3620387452) | Lazy-loading missing |
| PN003 | Network error recovery | DvChege | 10-Nov-2025 | Pass | - | Retried correctly |
| PN004 | Responsiveness under slow 3G | DvChege | 10-Nov-2025 | Pass | - | Functional, minor delay |

---

## 2. Execution Notes

- **Testing Method:** Manual testing on Chrome, Firefox, and Edge.  
- **Defect Tracking:** Failing test cases linked to **Defect Log (`defect log.md`)**.  
- **Evidence:** Screenshots and video demo saved under `/screenshots/` and `/videos/`.  
- **Traceability:** Each test case linked to corresponding functional requirements.  

---


