# Phase 2 - Test Case Design
**Team:** GTRs Testers  
**Application:** Bookstore App  
**Tester:** DvChege  
**Date:** November 2025  

| Test Case ID | Module | Test Objective | Pre-Condition | Test Steps | Expected Result | Status |
|--------------|---------|---------------|----------------|------------|----------------|--------|
| TC-001 | Login | Verify user can login with valid credentials | User account exists | 1. Open Login Page 2. Enter valid email/password 3. Click Login | Redirected to homepage/dashboard | Not Executed |
| TC-002 | Login | Verify error for invalid login | None | 1. Enter invalid credentials 2. Click Login | Error message: "Invalid email or password" | Not Executed |
| TC-003 | Book Catalog | Verify books display correctly | App running | 1. Navigate to Home 2. Scroll book list | Books should render with image, title, price | Not Executed |
| TC-004 | Book Catalog | Verify search functionality | Book list available | 1. Enter keyword in search bar 2. Click Search | Filtered results relevant to keyword | Not Executed |
| TC-005 | Cart | Verify adding a book to cart | User logged in | 1. Select a book 2. Click "Add to Cart" | Book appears in cart with quantity=1 | Not Executed |
| TC-006 | Cart | Verify updating cart quantity | Book already in cart | 1. Increase/Decrease quantity | Total updates correctly | Not Executed |
| TC-007 | Checkout | Verify checkout page loads | Items in cart | 1. Click Checkout | Checkout summary displayed | Not Executed |
| TC-008 | Payments | Verify payment with Paystack Test Mode | Checkout reached | 1. Click Pay 2. Enter test card details 3. Confirm | Payment Success confirmation displayed | Not Executed |
| TC-009 | Order Confirmation | Ensure order receipt shows after payment | Successful payment | After payment redirect | Order confirmation screen displays order ID | Not Executed |
| TC-010 | Logout | Verify user logout functionality | Logged in user | 1. Click Logout | Redirected to login page | Not Executed |
