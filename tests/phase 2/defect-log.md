# Phase 2 - Defect Log (Bookstore App)

## Team: GTRs Testers  
**Prepared By:** Emmaculate Mumbua  
**Date:** November 2025  
**Environment:** Chrome 129 / Firefox 128 , Windows 11, Android 

---

## Defect Table

| Bug ID | Summary | Severity / Priority | Environment | Affected FR Code(s) | Steps to Reproduce | Expected Result | Actual Result | Attachments / Notes |
|--------|---------|-------------------|-------------|-------------------|-----------------|----------------|---------------|-------------------|
| BUG-001 | “Buy Now” adds to cart without user feedback | Major | Firefox 128 | FR-O01 / FR-O02 | 1. Click "Buy Now" on a book | User sees confirmation / cart badge increments | Book added silently; user unaware | UI feedback missing; potential UX confusion |
| BUG-002 | Invalid city input accepted | Major | Chrome 129, Windows 11 | FR-O02 | 1. Enter city not in country → 2. Submit shipping form | Validation prevents submission | Form accepts invalid city | May cause shipping errors; backend does not validate input |
| BUG-003 | Book/author images not responsive | Major | Chrome 129, Android  | FR-O04 / FR-O01 | 1. Click book image or author in catalog | Opens book details | Nothing happens | Affects mobile usability; image click event not bound |
| BUG-004 | Cannot search by price | Major | Chrome 129, Windows 11 | FR-O01 | 1. Enter price range in search → 2. Apply filter | Results filtered by price | No filtering occurs | Filter functionality missing; affects purchase decisions |
| BUG-005 | Search bar at top center ineffective | Major | Chrome 129, Windows 11 | FR-O01 | 1. Type query in top search bar → 2. Press Enter | Catalog filters results | Results do not update | UX issue; search logic not hooked to backend |
| BUG-006 | Navigation limited to logo click | Major | Edge 128, Windows 11 | FR-O02 | 1. Attempt other navigation options | Any menu item returns to main page | Only logo clickable | Menu links broken; impacts site navigation |
| BUG-007 | Currency cannot be changed | Major | Chrome 129, Windows 11 | FR-O03 | 1. Attempt to select different currency | Display updates | Only default currency used | Payment display issue; may confuse international users |
| BUG-008 | Cannot view book details | Major | Chrome 129, Windows 11 | FR-O02 / FR-O04 | 1. Click a book in catalog → 2. Try to view details | Book details page opens | Clicking does nothing | Critical for catalog exploration; event not firing |
| BUG-009 | No coupon input available | Medium | Firefox 128, Windows 11 | FR-O02 | 1. Go to cart/checkout → 2. Look for coupon | Field available for input | Not present | Feature missing; affects promotional functionality |
| BUG-010 | Search results ignore diacritics | Medium | Chrome 129 | FR-O01 | 1. Search for book with accented letters | Book returned correctly | Book not found | Search algorithm not Unicode-aware; may miss valid results |
| BUG-011 | Lazy-loading images missing | Minor | Chrome 129, Android  | FR-X02 | 1. Load catalog → 2. Scroll | Images load lazily | All images load immediately | Performance issue; affects page load speed |
| BUG-012 | Notification badge not updated after mark-all-read | Minor / Low | Firefox 128, Windows 11 | FR-N02 | 1. Open notifications → 2. Click mark-all-read | Badge clears | Badge remains | Minor UX glitch; notification state not refreshed |
| BUG-013 | Stock race condition in mini-cart | Minor | Chrome 129, Windows 11 | FR-O01 | 1. Add item to cart → 2. Increase qty rapidly | Qty <= stock | Qty exceeds stock | Backend stock logic not enforcing constraints |
| BUG-014 | Return window off-by-one (day 8 accepted) | Minor | Edge 128, Windows 11 | FR-R01 | 1. Deliver order → 2. Attempt return on day 8 | Return rejected | Return accepted | Business rule violated; boundary condition bug |

---

## Defect Summary

- **Total Defects:** 14  
- **Critical / Major:** 8  
- **Minor / Medium:** 6  
- **Primary Impact Areas:** Catalog, Cart/Checkout, Payments, Navigation, Admin console  

---

## Functional Requirement Traceability

| FR Code | Description | Defects Linked |
|---------|------------|----------------|
| FR-O01 | Cart operations — add/remove/update with stock enforcement | BUG-001, BUG-002, BUG-003, BUG-004, BUG-011, BUG-013 |
| FR-O02 | Checkout wizard / validation | BUG-001, BUG-002, BUG-003, BUG-008, BUG-009 |
| FR-O03 | Payments — currency, Paystack init, exact cents | BUG-007 |
| FR-O04 | Catalog / Book detail | BUG-001, BUG-002, BUG-004, BUG-005, BUG-006 |
| FR-R01 | Returns — 7-day validation | BUG-014 |
| FR-N02 | Notifications — mark all read | BUG-012 |
| FR-X02 | Performance / Lazy images | BUG-011 |
```
