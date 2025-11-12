# Phase 2 
**Team:** GTRs Testers  
**Application:** Bookstore App  
**Tester:** DvChege  
**Date:** November 2025

---

<details>
<summary>1. UI Test Cases </summary>

| Test Case ID | Screen/Module | UI Element | Test Objective | Steps | Expected Result | Status |
|--------------|---------------|------------|----------------|-------|----------------|--------|
| UI-001 | Home Page | Book List Grid | Verify books are displayed in grid layout | 1. Open Home Page | Books appear in card layout with image + title + price | Not Executed |
| UI-002 | Home Page | Navbar | Check visibility, alignment, links, and hover effects | 1. Open Home Page 2. Inspect navbar items 3. Hover and click each | Navbar visible, items aligned, hover effect works, links navigate | Not Executed |
| UI-003 | Home Page | Search Bar | Verify visibility, placeholder, and input | 1. Open Home Page | Search bar visible, placeholder correct, allows typing | Not Executed |
| UI-004 | Home Page | Book Cards | Check card spacing, hover effects, clickable areas | 1. Observe cards 2. Hover on cards 3. Click card | Cards spaced evenly, hover highlights card, click navigates to details | Not Executed |
| UI-005 | Home Page | Category Filter | Verify visibility, clickable buttons | 1. Open Home Page | Filter buttons visible, clickable, filter books accordingly | Not Executed |
| UI-006 | Cart Icon | Badge Counter | Verify badge updates dynamically | 1. Add/remove items | Badge updates correctly | Not Executed |
| UI-007 | Buttons | Add to Cart | Verify visibility, hover, and active state | 1. Inspect button | Button visible, hover/active effect works, clickable | Not Executed |
| UI-008 | Checkout Page | Form Layout | Verify fields alignment and placeholder | 1. Open Checkout Page | Fields aligned, placeholder text correct | Not Executed |
| UI-009 | Footer | Links | Verify visibility and clickability | 1. Scroll to footer 2. Click links | Links visible and navigate correctly | Not Executed |
| UI-010 | Responsiveness | Home, Cart, Checkout | Verify layout adjusts to mobile/tablet | 1. Resize window/device | Layout adapts without overlap | Not Executed |
| UI-011 | Book Details | Details Page | Verify all elements | 1. Open book details | Title, author, price, description, Add to Cart visible | Not Executed |
| UI-012 | Tooltips | Buttons | Verify hover tooltips | 1. Hover over Add to Cart/Wishlist buttons | Tooltip displayed correctly | Not Executed |
| UI-013 | Error Messages | Forms | Verify inline validation | 1. Leave required field empty 2. Submit | Inline error message displayed | Not Executed |
| UI-014 | Images | Book Images | Verify image loads and fallback | 1. Open Home Page | Image visible or fallback if broken | Not Executed |
| UI-015 | Pagination/Scroll | Book List | Verify scroll or pagination works | 1. Scroll through book list | All books accessible, pagination correct | Not Executed |

</details>

<details>
<summary>2. Functional Test Cases</summary>

| Test Case ID | Module | Test Objective | Pre-Condition | Test Steps | Expected Result | Status |
|--------------|--------|----------------|---------------|------------|----------------|--------|
| TC-001 | Book Catalog | Display books correctly | App running | 1. Open Home Page 2. Scroll | Books appear with correct details | Not Executed |
| TC-002 | Book Catalog | Sorting by price/title | Books available | 1. Click sort dropdown | Books sorted correctly | Not Executed |
| TC-003 | Book Catalog | Filtering by category | Books available | 1. Select category filter | Only category books shown | Not Executed |
| TC-004 | Search | Search filters correctly | Books available | 1. Enter keyword 2. Click Search | Matching books displayed | Not Executed |
| TC-005 | Search | No results message | Books available | 1. Enter invalid keyword | “No results found” displayed | Not Executed |
| TC-006 | Search | Case-insensitive search | Books available | 1. Enter uppercase/lowercase keyword | Correct books displayed | Not Executed |
| TC-007 | Cart | Add book to cart | User logged in | 1. Select book 2. Click Add to Cart | Book appears in cart | Not Executed |
| TC-008 | Cart | Update quantity | Item in cart | 1. Increase/decrease quantity | Total updates correctly | Not Executed |
| TC-009 | Cart | Remove item | Item in cart | 1. Click Remove | Item removed, total updates | Not Executed |
| TC-010 | Cart | Empty cart checkout | Cart empty | 1. Click Checkout | Warning/error displayed, prevent checkout | Not Executed |
| TC-011 | Checkout | Load checkout page | Items in cart | 1. Click Checkout | Checkout summary visible | Not Executed |
| TC-012 | Payments | Successful payment | Checkout reached | 1. Pay via test card | Success screen with Order ID | Not Executed |
| TC-013 | Payments | Failed payment | Checkout reached | 1. Enter invalid card 2. Click Pay | Error message displayed | Not Executed |
| TC-014 | Order | Order receipt displayed | Payment completed | 1. Wait for redirect | Receipt with order details displayed | Not Executed |
| TC-015 | Wishlist | Add to wishlist | User logged in | 1. Click Add to Wishlist | Book added to wishlist | Not Executed |
| TC-016 | Wishlist | Remove from wishlist | Book in wishlist | 1. Remove book | Book removed | Not Executed |
| TC-017 | Account | Update profile | User logged in | 1. Edit profile 2. Save | Changes reflected correctly | Not Executed |
| TC-018 | Session | Session expiration | User logged in | 1. Stay idle 30 mins | User logged out, redirected to login | Not Executed |

</details>

<details>
<summary>3. Security / Edge Test Cases</summary>

| Test Case ID | Module | Test Objective | Pre-Condition | Test Steps | Expected Result | Status |
|--------------|--------|----------------|---------------|------------|----------------|--------|
| SE-002 | Input Validation | Prevent XSS in search/forms | Any input | 1. Enter script tag in input | Input sanitized, no code execution | Not Executed |
| SE-003 | Payment | Handle interrupted payment | Checkout reached | 1. Simulate payment disconnect | Show error, allow retry | Not Executed |
| SE-004 | Cart Limits | Max quantity enforcement | Book available | 1. Add more than allowed quantity | Display limit message | Not Executed |


</details>

<details>
<summary>4. Performance & Notifications</summary>

| Test Case ID | Module | Test Objective | Pre-Condition | Test Steps | Expected Result | Status |
|--------------|--------|----------------|---------------|------------|----------------|--------|
| PN-001 | Performance | Page load time | App running | 1. Open Home, Cart, Checkout | Pages load within acceptable time (<3s) | Not Executed |
| PN-002 | Notifications | Toast messages for actions | Any action | 1. Add/remove item 2. Wishlist action | Toast appears with correct message | Not Executed |
| PN-003 | Stress | Multiple cart additions | User logged in | 1. Rapidly add multiple books | Cart updates correctly without crash | Not Executed |
| PN-004 | Responsive | Mobile/tablet view | Resize window/device | 1. Check all pages | Layout adapts, no broken elements | Not Executed |

</details>

