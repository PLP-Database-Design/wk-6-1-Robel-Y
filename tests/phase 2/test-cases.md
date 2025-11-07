# Phase 2 Test Cases – Bookstore Application
**Team:** GTRs Testers  
**Tester:** DvChege  
**Date:** November 2025  

This document contains the UI and Functional test cases executed during Phase 2.

---

## 1. UI Test Cases

| TC ID | UI Element | Steps | Expected Result | Status |
|------|------------|--------|----------------|--------|
| UI001 | Homepage Layout | Open the homepage. | Page loads with header, search bar, and book grid. | Not Tested |
| UI002 | Book Cards Layout | Scroll through the book list. | Each book card displays: Image, Title, Author, Price, Button. | Not Tested |
| UI003 | Image Rendering | Inspect multiple book covers. | All images load without broken links. | Not Tested |
| UI004 | Search Bar UI | Observe search input box. | Search bar is visible, aligned, and usable. | Not Tested |
| UI005 | Responsive Layout | Resize browser to mobile width. | Book cards stack vertically without overlapping UI. | Not Tested |

---

## 2. Functional Test Cases

| TC ID | Feature | Precondition | Steps | Expected Result | Status |
|------|---------|--------------|--------|----------------|--------|
| FN001 | Load Book Catalog | Browser open | Navigate to homepage. | List of books loads successfully. | Not Tested |
| FN002 | Search – Exact Match | Homepage loaded | Search using full book title. | Matching book(s) appear. | Not Tested |
| FN003 | Search – Partial Match | Homepage loaded | Search using a partial title. | Relevant matches appear. | Not Tested |
| FN004 | Search – Case Insensitive | Homepage loaded | Search using lowercase / uppercase variations. | Same results regardless of typing case. | Not Tested |
| FN005 | Search No Results | Homepage loaded | Enter random text (ex: "zzzz"). | Display message: “No books found.” | Not Tested |
| FN006 | Clear Search Results | Search performed | Remove text in search bar. | Original full book list is shown. | Not Tested |
| FN007 | Buy Button Click | Book list visible | Click “Buy Now” on any book. | *No action occurs* (Feature not implemented yet). | Known Limitation |

---

## 3. Defect Log

| Defect ID | Module | Description | Steps to Reproduce | Expected Result | Actual Result | Severity | Status |
|-----------|--------|-------------|-------------------|----------------|---------------|----------|--------|
| D001 | Book Details Page | Clicking a book does not open details. | Click any book. | Book details page should open. | Nothing happens. | High | Open |
| D002 | Cart Feature | “Buy Now” button does not trigger any function. | Click “Buy Now”. | Should add to cart or start checkout. | No behavior. | Medium | Open |

---

## 4. Test Execution Summary

| Test Case ID | Date | Tester | Result (Pass/Fail) | Notes |
|--------------|------|--------|-------------------|-------|
| UI001 |  |  |  |  |
| UI002 |  |  |  |  |
| FN001 |  |  |  |  |
| FN002 |  |  |  |  |
| FN005 |  |  |  |  |
| FN007 |  |  |  | Known feature missing |

---

### ✅ End of Phase 2 Test Case Document
