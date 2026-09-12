# Test Execution Record

## Application
SauceDemo / Swag Labs

## Test Scope
The execution covered the main user journey from login through product browsing, cart management, checkout, order completion, and returning to the products page.

## Test Environment

The test execution was performed across two environments:

| Test Cases | Operating System | Browser |
|---|---|---|
| TC-001 to TC-019 | Windows (HP laptop) | Chrome |
| TC-020 to TC-025 | macOS (MacBook) | Chrome |

- Application: https://www.saucedemo.com/
- Testing Type: Manual Testing

## Environment Notes

- TC-001 through TC-019 were executed on an HP laptop running Windows.
- TC-020 through TC-025 were executed after switching to a MacBook running macOS.
- The same SauceDemo application and Chrome browser were used during the execution.
- The change of operating system occurred during the test execution cycle and is recorded to maintain an accurate execution history.

## Execution Summary

| Metric | Result |
|---|---:|
| Total Test Cases | 25 |
| Passed | 25 |
| Failed | 0 |
| Blocked | 0 |
| Pass Rate | 100% |

## Detailed Execution Results

| Test Case ID | Scenario | Status | Actual Result |
|---|---|---|---|
| TC-001 | Successful Login | PASS | Valid credentials successfully logged in and displayed the Products page with available products. |
| TC-002 | Invalid Password | PASS | Login was prevented and an incorrect username/password error was displayed. The user remained on the login page. |
| TC-003 | Invalid Username | PASS | Login was prevented and an incorrect username/password error was displayed. The user remained on the login page. |
| TC-004 | Empty Username | PASS | The application displayed the error message: "Epic sadface: Username is required." |
| TC-005 | Empty Password | PASS | The application displayed the error message: "Epic sadface: Password is required." |
| TC-006 | Inventory Products Display | PASS | The Products page displayed product names, prices, images, and Add to cart buttons. |
| TC-007 | Product Details | PASS | Selecting a product opened its details page with the product information and Add to cart option. |
| TC-008 | Add Product to Cart | PASS | The selected product was added to the cart and the cart count increased to 1. |
| TC-009 | Sort Products by Price | PASS | Products were successfully sorted by price from low to high. |
| TC-010 | Sort Products by Name | PASS | Products were successfully sorted alphabetically by name. |
| TC-011 | Product Appears in Cart | PASS | The selected product appeared in the cart with the expected product information. |
| TC-012 | Add Multiple Products | PASS | Two products were successfully added and the cart count displayed 2. |
| TC-013 | Remove Product from Cart | PASS | The selected product was removed and the remaining product stayed in the cart. |
| TC-014 | Product Information in Cart | PASS | Product name, price, and quantity in the cart matched the selected product information. |
| TC-015 | Continue Shopping | PASS | Continue Shopping returned the user to the Products page while retaining the selected product in the cart. |
| TC-016 | Proceed to Checkout | PASS | Selecting Checkout opened the Checkout: Your Information page with the required input fields. |
| TC-017 | Empty First Name | PASS | The application displayed the error message: "First Name is required." |
| TC-018 | Empty Last Name | PASS | The application displayed the error message: "Last Name is required." |
| TC-019 | Empty Postal Code | PASS | The application displayed the error message: "Postal Code is required." |
| TC-020 | Complete Checkout with Valid Information | PASS | Valid customer information was accepted and the user proceeded to the Checkout: Overview page. |
| TC-021 | Verify Checkout Overview | PASS | The overview displayed the selected product, quantity, payment information, shipping information, item total, tax, and total amount. |
| TC-022 | Verify Order Total | PASS | The displayed total of $32.39 matched the item total of $29.99 plus tax of $2.40. |
| TC-023 | Complete Order Successfully | PASS | Selecting Finish completed the order and displayed the Checkout: Complete! page with a thank-you message. |
| TC-024 | Verify Order Confirmation | PASS | The order confirmation page displayed the completion message, dispatch information, confirmation image, and Back Home button. |
| TC-025 | Return to Products After Order Completion | PASS | Selecting Back Home returned the user to the Products page. |

## Execution Observations

- All 25 executed test cases passed during manual execution.
- Login validation behaved as expected for valid and invalid credentials.
- Required checkout field validation displayed appropriate error messages.
- Product sorting, cart operations, and checkout calculations behaved as expected.
- The checkout flow successfully progressed from customer information to order completion.
- No failed test cases were recorded during this execution cycle.
- Defect and usability observations were documented separately following the exploratory and focused check.

## Execution Conclusion

The tested critical shopping journey from login through product selection, cart management, checkout, order completion, and return to the Products page completed successfully for the executed scenarios.

Exploratory testing, navigation/logout testing, browser behavior checks, and focused observation testing were also completed and documented. No confirmed functional defects were identified.

## Additional Navigation and State Checks

| Check | Actual Result | Status |
|---|---|---|
| Reset App State | After selecting Reset App State, the cart became empty. | PASS |
| Browser Refresh — Cart | The product remained in the cart after refreshing the browser. | PASS |
| Browser Refresh — Checkout Overview | The Checkout Overview and order information remained intact after refreshing. | PASS |
| Browser Back — Checkout Overview | Browser Back returned to the Checkout: Your Information page. | PASS |
| Logout → Browser Back | After logout, browser Back did not restore the Products page; the login page remained displayed. | PASS |
| Logout | Selecting Logout returned to the login page. | PASS |
| Browser Back — Product Details | Browser Back from Product Details returned to the Products page and loaded normally. | PASS |
