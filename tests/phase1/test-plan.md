# Bookstore Project - Test Plan Document
**Team Name:** GTRs Testers

## Introduction
This Test Plan document defines the testing strategy, objectives, scope, test environment, and responsibilities for the Bookstore application. The system is an e-commerce web application that allows users to browse books, add them to a cart, and simulate a checkout using the Paystack payment integration.

## Objectives
The main objective of testing is to ensure that all Bookstore application components function correctly, meet business requirements, and provide a smooth and error-free user experience. confusing behavior.

## Scope(In-scope)
Testing will mainly focus on these key features:

1. User registration and authentication
2. Book catalog and search functionality
3. Shopping cart and checkout process
4.  Inventory and order tracking
5. Payment integration (Paystack test mode)

## Out of Scope
Some parts of the system won’t be tested in this phase to keep things focused and manageable:

1. Real Paystack payments (only test mode will be used)  
2. Performance/load testing
3. Email notifications and password recovery  
4. Admin analytics and sales reports  
5. Mobile app version (only the web version is covered)

## Testing Types
We’ll use different types of testing to make sure all aspects of the app are covered:

- **Functional Testing** – To confirm each feature works as expected  
- **Integration Testing** – To verify that different modules work well together  
- **UI/UX Testing** – To check design consistency and usability  
- **Regression Testing** – To make sure fixes don’t break other parts of the app  
- **Acceptance Testing** – Final testing to confirm the system meets user needs  

## Test Environment
Testing will be done on a **local environment** using **Node.js** and **React**.  

- URL: `http://localhost:3000/`  
- Payment: Paystack (test mode only)  
- Test Data: Manually created sample data  
- Browser: Chrome, Firefox, and Edge (latest versions)  

## Test Deliverables
- Test Plan Document 
- Test Cases and Checklists
- Defect Log
- Final Test Report
- Project Board (GitHub) with test activities

## Entry and Exit Criteria

Entry Criteria:
- Repository setup completed
- Application runs locally
- Test environment configured

Exit Criteria:
- All planned test cases executed
- All critical and high-priority defects resolved
- Test report reviewed and approved

## Risks and Mitigation
| Risk | Impact | Mitigation |
|------|---------|------------|
| Unstable internet connection | May interrupt online calls | Use offline testing where possible and retry failed calls |
| Paystack test API downtime | Blocks checkout testing | Mock API responses to simulate transactions |
| Incomplete or outdated test data | May lead to inconsistent results | Refresh test data before execution |
| Time constraints | May reduce testing depth | Prioritize high-risk and core user flows first |

## Schedule
Phase 1: Planning & Setup – Due November 5, 2025
Phase 2: Test Design & Early Execution – Due November 11, 2025
Phase 3: Final Execution & Reporting – Due November 18, 2025

## Approval
Prepared By: DvChege
Date: November 3, 2025
Approved By: Robel Yihelu & Emmaculate Mumbua 

---
