# Bookstore Application – Phase 1 Requirements & System Overview

## 1. Introduction
The Bookstore Web Application allows users to browse a collection of books displayed on the homepage. Users can search for books by title using the built-in search bar. The system currently operates without authentication, cart system, or administrative dashboard.

This document outlines the key requirements gathered during Phase 1 and forms the basis for test planning and execution in Phase 2.

## 2. System Objectives
- Display a list of books to users in a clear and visually appealing layout.
- Allow users to search for books using a search field.
- Ensure consistent UI behavior and responsiveness across supported devices.

## 3. Current Functionality (Scope of Phase 1)
| Feature | Description | Status |
|--------|-------------|--------|
| Book Listing | Displays all available books on homepage with image, name, author, and price. | Implemented |
| Book Search | Allows users to search by book title. | Implemented |
| Product Detail Page | View more information about a book. | Not Implemented (Out of Scope) |
| Cart and Checkout | Add to cart, remove, order checkout. | Not Implemented (Future Phase) |
| User Authentication | Login / Register | Not Implemented |
| Admin Dashboard | Manage books, inventory, sales. | Not Implemented |

## 4. Non-Functional Requirements
- UI must be user-friendly and fast-loading.
- Application should follow a clean and minimalist design style.
- Search should provide results instantly without page reload.

## 5. Tools and Technologies
- **Frontend:** React / HTML / CSS (as seen in UI)
- **Data Source:** Mock Data JSON (Assumed from screenshots)
- **Hosting (Future):** To be determined

## 6. Conclusion
Phase 1 successfully delivered the core browsing and search functionalities. Future phases will expand the system to include cart, authentication, and admin management.
