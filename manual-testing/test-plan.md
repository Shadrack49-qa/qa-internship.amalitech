# Risk-Based Test Plan

## 1. Project Overview

This test plan defines the approach for manually testing the SauceDemo / Swag Labs web application.

The purpose of the testing is to verify that the application's major user journeys work as expected and to identify defects, usability issues, and risks that could affect users.

## 2. Application Under Test

**Application:** SauceDemo / Swag Labs

**URL:** https://www.saucedemo.com/

## 3. Testing Objectives

The objectives of this testing are to:

- Verify that users can successfully log in.
- Verify that products are displayed correctly.
- Verify that users can view and interact with product information.
- Verify that users can sort products.
- Verify that users can add and remove products from the cart.
- Verify that users can complete the checkout process.
- Verify that users can log out successfully.
- Identify functional defects and usability issues.
- Perform exploratory testing to discover issues outside the scripted test cases.

## 4. Scope

### In Scope

The following areas will be tested:

- Login and authentication
- Product inventory
- Product details
- Product sorting
- Shopping cart
- Checkout
- Order completion
- Navigation
- Logout
- Basic responsive/browser behaviour
- Exploratory testing

### Out of Scope

The following areas are outside the scope of this assignment:

- Backend/server infrastructure testing
- Database testing
- Performance/load testing
- Security penetration testing
- Source code testing
- Payment gateway integration with real financial transactions

## 5. Testing Approach

The testing will use a risk-based manual testing approach.

The following testing techniques will be applied:

- Functional testing
- Positive testing
- Negative testing
- Boundary testing
- State-based testing
- Exploratory testing
- Usability testing
- Basic browser/responsive testing

Critical user journeys will receive higher testing priority.

## 6. Risk Assessment

| Area | Risk Level | Reason |
|---|---|---|
| Login | High | Users must authenticate before accessing the application |
| Product Inventory | Medium | Incorrect product information can affect purchasing decisions |
| Product Sorting | Medium | Incorrect sorting can reduce usability |
| Shopping Cart | High | Cart errors can result in incorrect orders |
| Checkout | High | Checkout is a critical business flow |
| Order Completion | High | Users need confirmation that their order was successfully processed |
| Navigation | Medium | Navigation problems can prevent users from completing tasks |
| Logout | Medium | Users should be able to safely end their session |

## 7. Test Environment

**Operating System:** Windows

**Browser:** Google Chrome

**Application:** SauceDemo / Swag Labs

## 8. Entry Criteria

Testing can begin when:

- The application is accessible.
- The main application pages can be loaded.
- Test credentials are available.
- The test environment is ready.

## 9. Exit Criteria

Testing will be considered complete when:

- Planned high-priority scenarios have been executed.
- At least 18 detailed test cases have been executed.
- Test results have been recorded.
- Identified defects or quality observations have been documented.
- Exploratory testing has been completed.
- Evidence has been collected where applicable.
- A release recommendation has been made.

## 10. Deliverables

The testing project will produce:

- Risk-based test plan
- Test scenarios
- Detailed test cases
- Test execution results
- Defect reports / quality observations
- Exploratory testing session notes
- Evidence screenshots
- Final release recommendation