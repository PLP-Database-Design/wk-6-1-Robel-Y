# Defect Log – Bookstore Application (Phase 3)

**Team:** GTRs Testers  
**Prepared By:** Emmaculate Mumbua  
**Date:** November 2025  
**Environment:** Chrome 129 / Firefox 128 / Windows 11  / Android 12  

---

## 1. Defect Table

| Defect ID | Summary | Severity | Priority | Environment | Steps to Reproduce | Expected Result | Actual Result | Status | Notes |
|------------|----------|-----------|-----------|--------------|--------------------|----------------|----------------|---------|--------|
| BUG-001 | “Buy Now” adds to cart silently | Major | High | Firefox 128 | 1. Click “Buy Now” | User gets confirmation message | Book added silently | Open | Logged by DvChege |
| BUG-002 | Invalid city input accepted in checkout | Major | High | Chrome 129 | 1. Enter random city → 2. Submit | Validation prevents submission | Form accepts invalid data | Open | Logged by Emmaculate |
| BUG-003 | Some book/author images fail on Android | Major | Medium | Chrome 129, Android | 1. Load catalog | All images display | Some missing | Open | Linked to UI003 |
| BUG-004 | Price filter not functioning | Major | High | Chrome 129, Windows 11 | 1. Search by price | Books filtered accordingly | No filter applied | Open | Linked to TC003 |
| BUG-005 | Search bar not responsive on Enter | Major | Medium | Chrome 129, Windows 11 | 1. Type query → press Enter | Search executes | No response | Open | Linked to UI004 |
| BUG-007 | Currency cannot be changed | Major | Medium | Chrome 129, Windows 11 | 1. Try changing currency | Currency updates | Stuck on default | Open | Linked to TC004 |
| BUG-008 | Book details not viewable | Major | High | Chrome 129, Windows 11 | 1. Click book card | Details page opens | No response | Open | Linked to TC002 |
| BUG-009 | Coupon field missing on checkout | Medium | Medium | Firefox 128, Windows 11 | 1. Go to checkout | Coupon field visible | Not present | Open | Linked to TC005 |
| BUG-011 | Lazy-loading not implemented | Minor | Low | Chrome 129, Android 12 | 1. Scroll book catalog | Lazy-load images | All load immediately | Open | Linked to PN002 |

---

## 2. Summary

- **Total Defects:** 9  
- **Major:** 6  
- **Minor:** 3  
- **Open Defects:** 9  
- **Closed Defects:** 0  
- **Fixed in Next Phase:** Scheduled for Patch 1.1  

---

## 3. Recommendations

- Add proper UI feedback after “Buy Now” action.  
- Implement validation for checkout city input.  
- Enable lazy-loading and improve image optimization.  
- Expand search function to include all metadata (title, price, author).  

---

**End of Defect Log**

