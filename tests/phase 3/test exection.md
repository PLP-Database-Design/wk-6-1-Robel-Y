# Phase 3 – Test Execution Report  
**Team:** GTRs Testers  
**Application:** Bookstore App  
**Tester:** DvChege  
**Date:** November 2025  

---

## 1. Objective
This document records the actual execution of all UI and functional test cases for the Bookstore Application. Evidence is captured through screenshots demonstrating application behavior during testing.

---

## 2. Test Execution Summary

| Test Case ID | Module | Test Description | Expected Result | Actual Result | Status | Evidence |
|---------------|---------|------------------|-----------------|----------------|---------|-----------|
| TC01 | Book Listing | Verify that all books are displayed on the home page | All available books appear with image, title, author, and price | Displayed correctly | ✅ Pass | Screenshot_1 |
| TC02 | Book Details | Verify that clicking “Buy Now” displays book details | Details of the selected book appear | Displayed correctly | ✅ Pass | Screenshot_2 |
| TC03 | Cart | Verify that items can be added to the cart and subtotal updates correctly | Cart updates with new item and recalculates subtotal | Works as expected | ✅ Pass | Screenshot_3 |
| TC04 | Cart | Verify that the “Remove” button deletes selected item | Item removed and subtotal updated | Item removed but subtotal delayed | ❌ Fail | Screenshot_3 |
| TC05 | Checkout | Verify that all shipping fields accept valid input | User can enter all fields without error | Works correctly | ✅ Pass | Screenshot_4 |
| TC06 | Checkout | Verify that empty required fields show validation errors | System should display “Field required” message | No error shown | ❌ Fail | Screenshot_4 |
| TC07 | Payment | Verify that clicking “Next” moves to payment section | Payment page loads | Displayed correctly | ✅ Pass | Screenshot_5 |

---

## 3. Execution Evidence
**Evidence Screenshots:**  
- Screenshot_1 → Book Listing Page  
- Screenshot_2 → Book Details Page  
- Screenshot_3 → Cart Page  
- Screenshot_4 → Checkout Page  
- Screenshot_5 → Payment Navigation  

*(Screenshots correspond to the images uploaded during testing.)*

---

## 4. Summary
Out of 7 total test cases executed, **5 passed** and **2 failed**. Failed cases were logged for review in the defect log.  
The system shows good functional stability with minor validation issues.
