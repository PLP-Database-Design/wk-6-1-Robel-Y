# Test Case Design Document

## Project Name: Bookstore App  
## Team Name: GTRs Testers  
## Phase: Phase 2 – Test Planning and Design  
## Author: DvChege  
## Date: November 2025  

---

## 1. Introduction
This Test Case Design document defines the initial test cases for the **Bookstore Application**.  
Since the system does **not include user login or admin access**, all interactions occur under **guest access**.  

This document focuses on catalog browsing, shopping cart functionality, checkout flow, and product search features.

---

## 2. Test Objectives
- Validate that the core bookstore functionalities work correctly without authentication.
- Ensure a smooth user experience through browsing, searching, selecting products, and completing checkout.
- Provide structured and traceable test cases that guide both manual and automation testing in later phases.

---

## 3. Test Case Summary

| Test Case ID | Feature / Module | Test Steps | Expected Result | Priority |
|--------------|-----------------|------------|----------------|----------|
| TC001 | Guest Access | Open the Bookstore website | Homepage loads successfully with navigation and featured products visible | High |
| TC002 | Product Catalog | Navigate to the catalog section | All products display correctly with name, price, and image | High |
| TC003 | Product Catalog | Click on a product item | Product detail page displays accurate title, description, image, and price | Medium |
| TC004 | Shopping Cart | Add a product to cart from product page | Cart updates and displays correct quantity and subtotal | High |
| TC005 | Shopping Cart | Add multiple products to cart | Cart lists each item separately with accurate totals | Medium |
| TC006 | Shopping Cart | Remove an item from cart | Item is removed and total cost updates accordingly | High |
| TC007 | Checkout | Proceed to checkout and fill required details | Order is placed successfully and confirmation message is displayed | High |
| TC008 | Checkout Validation | Attempt checkout with missing required fields | Error message displayed prompting the user to complete missing fields | High |
| TC009 | Search | Search for an existing product name | Matching product(s) appear in search results | Medium |
| TC010 | Search | Search for a product that does not exist | Message displayed: “No results found” | Low |
| TC011 | Session Handling | Close and reopen browser | Cart resets (guest session does not persist data unless session storage is implemented) | Medium |

> **Removed Test Cases:** Login & Admin Access — not applicable for this system.

---

## 4. Traceability
Each test case corresponds to functional requirements gathered in Phase 1.  
This ensures full coverage of core business workflows.

---

## 5. Review and Approval

| Reviewer | Role | Approval Status | Date |
|---------|------|----------------|------|
| Robel Yihelu | QA Lead | Approved | November 2025 |
| Emmaculate Mumbua | Documentation Lead | Approved | November 2025 |

---
