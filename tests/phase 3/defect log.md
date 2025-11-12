# Phase 3 – Defect Log  
**Team:** GTRs Testers  
**Application:** Bookstore App  
**Tester:** DvChege  
**Date:** November 2025  

---

## 1. Objective
To record and track all identified defects from the test execution phase, along with their severity, priority, and resolution status.

---

## 2. Defect Table

| Defect ID | Module | Description | Steps to Reproduce | Expected Result | Actual Result | Severity | Priority | Status | Assigned To |
|------------|---------|-------------|--------------------|-----------------|----------------|-----------|-----------|----------|--------------|
| DEF-01 | Cart | Subtotal not updating immediately after removing an item | 1. Add multiple books to cart<br>2. Remove one<br>3. Check subtotal | Subtotal should update instantly | Subtotal updates only after refresh | Medium | P2 | Open | Developer 1 |
| DEF-02 | Checkout | Required field validation missing | 1. Leave fields empty<br>2. Click “Next” | Error message “Field required” should appear | No validation message shown | High | P1 | Open | Developer 2 |
| DEF-03 | Cart | Quantity accepts non-numeric input | 1. Add book<br>2. Enter letters in quantity field | Only numbers should be accepted | Accepts letters | Low | P3 | Resolved | Developer 3 |

---

## 3. Defect Summary
- **Total Defects Logged:** 3  
- **Resolved Defects:** 1  
- **Pending Defects:** 2  
- **Critical (High Severity):** 1  

Follow-up retesting is recommended once open defects are fixed.
