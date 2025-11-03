# Test Case Design Document

** Project Name:** Bookstore App  
** Team Name:** GTRs Testers
** Phase:** Phase 2 – Test Planning and Design  
** Author:** DvChege  
** Date:** November 2025  


## 1. Introduction
This Test Case Design document defines the initial test cases for the **Bookstore application**.  
It focuses on verifying the main functionalities such as catalog browsing, cart management, checkout process, and administrative access.  

These test cases are based on the requirements identified during Phase 1 and will be used for manual testing in the following project phases.

## 2. Test Objectives
The purpose of this document is to provide clear, structured, and traceable test cases to ensure that the application's main user journeys and features are functioning as expected.  

This document also serves as a foundation for test execution, defect tracking, and reporting in later stages of the project.

## 3. Test Case Summary

| Test Case ID | Feature / Module | Test Steps | Expected Result | Priority |
|---------------|------------------|-------------|------------------|-----------|
| **TC001** | User Login | Navigate to login page, enter valid credentials, click **Login** | User successfully logs in and is redirected to homepage | High |
| **TC002** | User Login | Enter invalid password and click **Login** | Error message displayed: *"Invalid credentials"* | High |
| **TC003** | Product Catalog | Open catalog page | All products load correctly with name, price, and image | High |
| **TC004** | Product Catalog | Click on a product item | Product detail page opens with accurate data | Medium |
| **TC005** | Shopping Cart | Add product to cart | Cart updates and displays correct total | High |
| **TC006** | Shopping Cart | Remove item from cart | Item is removed and total updates correctly | Medium |
| **TC007** | Checkout | Proceed to checkout with valid details | Order is placed successfully | High |
| **TC008** | Checkout | Leave a required field empty and submit | Error validation message displayed | High |
| **TC009** | Search | Search for an existing product | Product appears in search results | Medium |
| **TC010** | Search | Search for a non-existing product | “No results found” message displayed | Low |
| **TC011** | Admin Access | Try to access `/admin` without logging in | Access denied or redirected to login page | High |
| **TC012** | Admin Access | Login as admin and navigate to `/admin` | Admin dashboard loads successfully with all controls visible | High |

## 4. Traceability
Each test case is linked to specific **functional requirements** and **acceptance criteria**.  
Traceability ensures that every user story and business rule has corresponding test coverage, reducing the risk of untested functionality.

## 5. Review and Approval
This document has been prepared by **DvChege** and reviewed by the **QA Team**.  
It serves as the baseline for test execution in the next phase.

| Reviewer | Role | Approval Status | Date |
|-----------|------|------------------|------|
| Robel Yihelu | QA Lead | Approved | November 2025 |
| Emmaculate Mumbua | Documentation Lead | Approved | November 2025 |

---
