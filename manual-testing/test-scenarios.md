# Test Scenarios

## 1. Login and Authentication

| ID | Test Scenario | Priority |
|---|---|---|
| TS-001 | Verify that a user can log in with valid credentials | High |
| TS-002 | Verify that login fails when an incorrect password is entered | High |
| TS-003 | Verify that login fails when an invalid username is entered | High |
| TS-004 | Verify that login fails when the username field is empty | High |
| TS-005 | Verify that login fails when the password field is empty | High |

## 2. Product Inventory

| ID | Test Scenario | Priority |
|---|---|---|
| TS-006 | Verify that the inventory page displays available products | High |
| TS-007 | Verify that a user can view product details | Medium |
| TS-008 | Verify that a user can add a product to the cart from the inventory page | High |
| TS-009 | Verify that a user can sort products by price | Medium |
| TS-010 | Verify that a user can sort products by product name | Medium |

## 3. Shopping Cart

| ID | Test Scenario | Priority |
|---|---|---|
| TS-011 | Verify that an added product appears in the shopping cart | High |
| TS-012 | Verify that a user can add multiple products to the cart | High |
| TS-013 | Verify that a user can remove a product from the cart | High |
| TS-014 | Verify that the cart displays the correct product information | High |
| TS-015 | Verify that a user can continue shopping after viewing the cart | Medium |

## 4. Checkout

| ID | Test Scenario | Priority |
|---|---|---|
| TS-016 | Verify that a user can proceed from the cart to checkout | High |
| TS-017 | Verify that checkout cannot proceed when the first name is empty | High |
| TS-018 | Verify that checkout cannot proceed when the last name is empty | High |
| TS-019 | Verify that checkout cannot proceed when the postal code is empty | High |
| TS-020 | Verify that a user can successfully enter valid checkout information | High |
| TS-021 | Verify that the checkout overview displays the selected product and price correctly | High |
| TS-022 | Verify that a user can successfully complete an order | High |

## 5. Navigation and Logout

| ID | Test Scenario | Priority |
|---|---|---|
| TS-023 | Verify that a user can navigate between the inventory page and shopping cart | Medium |
| TS-024 | Verify that a user can successfully log out | High |
| TS-025 | Verify that a logged-out user cannot access protected application pages through normal navigation | High |