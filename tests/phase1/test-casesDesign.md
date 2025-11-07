# Phase 1 – Test Case Design Document
## Project: Bookstore Application  
## Team: GTRs Testers  
## Date: November 2025  
## Author: DvChege

---

### 1. Introduction
This document outlines the initial test cases for the Bookstore Web Application as implemented in Phase 1. The current application allows users to browse a list of books and search for books by title. No login, checkout, or admin features are present in this phase.

---

### 2. Test Scope (Phase 1)
| Feature | Included | Notes |
|--------|:--------:|------|
| Book Catalog Listing | ✅ | Fully implemented |
| Search Function | ✅ | Fully implemented |
| Product Detail Page | ❌ | Not yet implemented |
| Cart & Checkout | ❌ | Not part of Phase 1 |
| User Login/Registration | ❌ | Not part of Phase 1 |
| Admin Dashboard | ❌ | Not part of Phase 1 |

---

### 3. Test Case Summary

| Test Case ID | Feature | Precondition | Test Steps | Expected Result | Status | Priority |
|--------------|---------|--------------|------------|----------------|--------|----------|
| TC001 | Homepage Load | Browser open | 1. Navigate to the homepage URL. | Homepage loads successfully with book catalog visible. | To be Tested | High |
| TC002 | Book Listing Display | Homepage loaded | 1. Verify each book card shows: **Image, Title, Author, Price, Buy Now button**. | All book cards display complete correct information. | To be Tested | High |
| TC003 | Book Count Verification | Homepage loaded | 1. Count number of books displayed. 2. Compare with expected list in data. | Number of displayed books matches book dataset. | To be Tested | Medium |
| TC004 | Search – Exact Match | Homepage loaded | 1. Type full title of an existing book in Search bar. | Only the matching book(s) appear. | To be Tested | High |
| TC005 | Search – Partial Text Match | Homepage loaded | 1. Enter partial book title (e.g., “Mock” for *To Kill a Mockingbird*). | Books with matching partial text appear. | To be Tested | Medium |
| TC006 | Search – Case Sensitivity | Homepage loaded | 1. Type book title in different letter casing (e.g., *gatsby*, *GATSBY*). | Search returns the same result regardless of case. | To be Tested | Medium |
| TC007 | Search – No Match | Homepage loaded | 1. Enter random text that does not match any book. | Display message: **“No books found matching your search.”** | To be Tested | Low |
| TC008 | Search Clear Function | A search has been performed | 1. Clear the search input. | Full list of books is displayed again. | To be Tested | Medium |
| TC009 | UI Responsiveness | App opened in desktop | 1. Resize screen to mobile width. | Layout adjusts, books remain visible and readable. | To be Tested | Low |

---

### 4. Test Environment
| Component | Details |
|----------|---------|
| Browser | Chrome (Latest), Firefox (Optional) |
| Display | Desktop and Mobile View |
| Data Source | Static/MOCK book list (imported data) |

---

### 5. Conclusion
These test cases validate the current capabilities delivered in Phase 1. Future phases will include additional test cases for cart operations, checkout process, authentication, and admin role functionality.

---
