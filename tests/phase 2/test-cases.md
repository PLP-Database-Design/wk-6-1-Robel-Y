# Phase 2 - Test Case Design & Execution  
**Team:** GTRs Testers  
**Application:** Bookstore App  
**Tester:** DvChege  
**Date:** November 2025  


---

## 1. UI Test Cases

| Test Case ID | Screen/Module | UI Element | Test Objective | Steps | Expected Result | Status |
|--------------|---------------|------------|----------------|-------|----------------|--------|
| UI-001 | Home Page | Book List Grid | Verify books are displayed in grid layout | 1. Open Home Page | Books appear in card layout with image + title + price | Not Executed |
| UI-002 | Home Page | Navbar | Check whether navbar is visible and correctly aligned | 1. Open Home Page | Navbar appears at top and is readable | Not Executed |
| UI-003 | Home Page | Search Bar | Verify search input visibility | 1. Open Home Page | Search bar is visible and allows typing | Not Executed |
| UI-004 | Home Page | Book Cards | Check card spacing and readability | 1. Observe book cards | Cards are spaced evenly and not overlapping | Not Executed |
| UI-005 | Cart Icon | Cart Badge | Verify badge updates when cart has items | 1. Add item to cart | Badge increments to reflect cart count | Not Executed |
| UI-006 | Cart Page | Item table/list | Ensure cart items display properly | 1. Open Cart Page | Items show image + price + quantity buttons | Not Executed |
| UI-007 | Buttons | Add to Cart Button | Confirm button visibility and usability | 1. Check any book card | Button is clear, clickable and styled | Not Executed |
| UI-008 | Checkout Page | Form layout | Verify address/payment details display correctly | 1. Proceed to checkout | Fields aligned and readable | Not Executed |


---

## 2. Functional Test Case Design

| Test Case ID | Module | Test Objective | Pre-Condition | Test Steps | Expected Result | Status |
|--------------|---------|---------------|---------------|------------|----------------|--------|

| TC-001 | Login | Verify login fails for invalid credentials | None | 1. Enter invalid credentials 2. Click Login | Error message appears | Not Executed |
| TC-002 | Book Catalog | Verify books display correctly | App running | 1. Open Home Page 2. Scroll book list | Books show with correct details | Not Executed |
| TC-003 | Search | Verify search functionality filters correctly | Books available | 1. Enter search keyword 2. Click Search | Only matching books appear | Not Executed |
| TC-004 | Cart | Verify adding a book to cart adds correct entries | User logged in | 1. Select any book 2. Click Add to Cart | Book appears in cart | Not Executed |
| TC-005 | Cart | Verify changing quantity updates total | Item already in cart | 1. Change quantity from 1→2 | Total updates correctly | Not Executed |
| TC-006 | Checkout | Verify checkout page loads | Items in cart | 1. Click Checkout | Checkout summary appears | Not Executed |
| TC-007 | Payments | Verify payment with Paystack test mode | Checkout reached | 1. Click Pay 2. Enter test card 3. Confirm | Payment Success screen appears | Not Executed |
| TC-008 | Order Confirmation | Verify order receipt displays | Payment completed | 1. Wait for redirect | Receipt displays with Order ID | Not Executed |
| TC-009 | Logout | Verify logout redirects user | Logged in user | 1. Click Logout | User returns to login page | Not Executed |


---

## 3. Test Execution Report

| Test Case ID | Executed By | Date Executed | Result (Pass/Fail) | Notes |
|--------------|-------------|---------------|--------------------|-------|
| UI-001 | | | | |
| UI-002 | | | | |
| UI-003 | | | | |
| UI-004 | | | | |
| UI-005 | | | | |
| UI-006 | | | | |
| UI-007 | | | | |
| UI-008 | | | | |
| UI-009 | | | | |
| UI-010 | | | | |
| TC-001 | | | | |
| TC-002 | | | | |
| TC-003 | | | | |
| TC-004 | | | | |
| TC-005 | | | | |
| TC-006 | | | | |
| TC-007 | | | | |
| TC-008 | | | | |
| TC-009 | | | | |
| TC-010 | | | | |

---

