# Detailed Test Cases

## TC-001 — Successful Login

| Field | Details |
|---|---|
| Test Case ID | TC-001 |
| Scenario ID | TS-001 |
| Title | Verify that a user can log in with valid credentials |
| Priority | High |
| Preconditions | User is on the SauceDemo login page |
| Test Data | Username: `standard_user`<br>Password: `secret_sauce` |

### Test Steps

1. Enter `standard_user` in the Username field.
2. Enter `secret_sauce` in the Password field.
3. Click the Login button.

### Expected Result

The user should be successfully authenticated and redirected to the Products page, where the product inventory should be displayed.

### Actual Result

The user was successfully taken to the Products page and the products were displayed.

### Status

**PASS**

## TC-002 — Invalid Password

| Field | Details |
|---|---|
| Test Case ID | TC-002 |
| Scenario ID | TS-002 |
| Title | Verify that login fails when an incorrect password is entered |
| Priority | High |
| Preconditions | User is on the SauceDemo login page |
| Test Data | Username: `standard_user`<br>Password: `secretsauce` |

### Test Steps

1. Enter `standard_user` in the Username field.
2. Enter `secretsauce` in the Password field.
3. Click the Login button.

### Expected Result

The application should prevent the user from logging in and display an appropriate error message indicating that the username or password is incorrect.

### Actual Result

The application prevented login, displayed an error message indicating an incorrect username or password, and kept the user on the login page.

### Status

**PASS**

## TC-003 — Invalid Username

| Field | Details |
|---|---|
| Test Case ID | TC-003 |
| Scenario ID | TS-003 |
| Title | Verify that login fails when an invalid username is entered |
| Priority | High |
| Preconditions | User is on the SauceDemo login page |
| Test Data | Username: `standarduser`<br>Password: `secret_sauce` |

### Test Steps

1. Enter `standarduser` in the Username field.
2. Enter `secret_sauce` in the Password field.
3. Click the Login button.

### Expected Result

The application should prevent the user from logging in and display an appropriate error message indicating that the username or password is incorrect.

### Actual Result

The application prevented login, displayed an error message indicating an incorrect username or password, and kept the user on the login page.

### Status

**PASS**

## TC-004 — Empty Username

| Field | Details |
|---|---|
| Test Case ID | TC-004 |
| Scenario ID | TS-004 |
| Title | Verify that login fails when the username field is empty |
| Priority | High |
| Preconditions | User is on the SauceDemo login page |
| Test Data | Username: *(empty)*<br>Password: `secret_sauce` |

### Test Steps

1. Leave the Username field empty.
2. Enter `secret_sauce` in the Password field.
3. Click the Login button.

### Expected Result

The application should prevent the user from logging in and display an appropriate validation message indicating that the username is required.

### Actual Result

The application prevented login and displayed the error message: **"Epic sadface: Username is required."**

### Status

**PASS**

## TC-005 — Empty Password

| Field | Details |
|---|---|
| Test Case ID | TC-005 |
| Scenario ID | TS-005 |
| Title | Verify that login fails when the password field is empty |
| Priority | High |
| Preconditions | User is on the SauceDemo login page |
| Test Data | Username: `standard_user`<br>Password: *(empty)* |

### Test Steps

1. Enter `standard_user` in the Username field.
2. Leave the Password field empty.
3. Click the Login button.

### Expected Result

The application should prevent the user from logging in and display an appropriate validation message indicating that the password is required.

### Actual Result

The application prevented login and displayed the error message: **"Epic sadface: Password is required."**

### Status

**PASS**

## TC-006 — Inventory Products Display

| Field         | Details                                                    |
| ------------- | ---------------------------------------------------------- |
| Test Case ID  | TC-006                                                     |
| Scenario ID   | TS-006                                                     |
| Title         | Verify that the inventory page displays available products |
| Priority      | High                                                       |
| Preconditions | User has successfully logged in with valid credentials     |
| Test Data     | Username: `standard_user`<br>Password: `secret_sauce`      |

### Test Steps

1. Log in using `standard_user` and `secret_sauce`.
2. Navigate to the Products page.
3. Verify that the Products heading is visible.
4. Verify that multiple products are displayed.
5. Verify that each product has a name, price, image, and Add to cart button.

### Expected Result

The Products page should display the Products heading and available products. Each product should have a product name, price, image, and Add to cart button.

### Actual Result

The Products heading was visible, multiple products were displayed, and each product had a name, price, image, and Add to cart button.

### Status

**PASS**

## TC-007 — Product Details

| Field         | Details                                               |
| ------------- | ----------------------------------------------------- |
| Test Case ID  | TC-007                                                |
| Scenario ID   | TS-007                                                |
| Title         | Verify that a user can view product details           |
| Priority      | Medium                                                |
| Preconditions | User is logged in and is on the Products page         |
| Test Data     | Username: `standard_user`<br>Password: `secret_sauce` |

### Test Steps

1. Log in using `standard_user` and `secret_sauce`.
2. From the Products page, select any product.
3. Click on the product name or image.
4. Verify that the product details page is displayed.
5. Verify the product name, image, description, price, Add to cart button, and Back to products button.

### Expected Result

The selected product's details page should open and display the product name, image, description, price, Add to cart button, and Back to products button.

### Actual Result

The product details page opened successfully and displayed the product name, image, description, price, Add to cart button, and Back to products button.

### Status

**PASS**

## TC-008 — Add Product to Cart

| Field         | Details                                                                  |
| ------------- | ------------------------------------------------------------------------ |
| Test Case ID  | TC-008                                                                   |
| Scenario ID   | TS-008                                                                   |
| Title         | Verify that a user can add a product to the cart from the inventory page |
| Priority      | High                                                                     |
| Preconditions | User is logged in and on the Products page                               |
| Test Data     | Username: `standard_user`<br>Password: `secret_sauce`                    |

### Test Steps

1. Select a product from the Products page.
2. Click the **Add to cart** button.
3. Observe the selected product's button.
4. Observe the shopping cart icon.

### Expected Result

The selected product should be added to the shopping cart. The Add to cart button should change to Remove, and the cart should display a count of 1.

### Actual Result

After clicking **Add to cart**, the button changed to **Remove**, and the shopping cart count changed to **1**.

### Status

**PASS**

## TC-009 — Sort Products by Price

| Field         | Details                                               |
| ------------- | ----------------------------------------------------- |
| Test Case ID  | TC-009                                                |
| Scenario ID   | TS-009                                                |
| Title         | Verify that a user can sort products by price         |
| Priority      | Medium                                                |
| Preconditions | User is logged in and on the Products page            |
| Test Data     | Username: `standard_user`<br>Password: `secret_sauce` |

### Test Steps

1. Navigate to the Products page.
2. Click the Sort dropdown.
3. Select **Price (low to high)**.
4. Observe the prices of the displayed products.

### Expected Result

The products should be arranged in ascending order, from the lowest price to the highest price.

### Actual Result

The products were arranged from the lowest price to the highest price.

### Status

**PASS**

## TC-010 — Sort Products by Name

| Field         | Details                                               |
| ------------- | ----------------------------------------------------- |
| Test Case ID  | TC-010                                                |
| Scenario ID   | TS-010                                                |
| Title         | Verify that a user can sort products by product name  |
| Priority      | Medium                                                |
| Preconditions | User is logged in and on the Products page            |
| Test Data     | Username: `standard_user`<br>Password: `secret_sauce` |

### Test Steps

1. Navigate to the Products page.
2. Click the Sort dropdown.
3. Select **Name (A to Z)**.
4. Observe the product names from top to bottom.

### Expected Result

The products should be arranged alphabetically from A to Z.

### Actual Result

The product names were arranged alphabetically from A to Z.

### Status

**PASS**

## TC-011 — Product Appears in Cart

| Field         | Details                                                   |
| ------------- | --------------------------------------------------------- |
| Test Case ID  | TC-011                                                    |
| Scenario ID   | TS-011                                                    |
| Title         | Verify that an added product appears in the shopping cart |
| Priority      | High                                                      |
| Preconditions | User is logged in and has added a product to the cart     |
| Test Data     | Username: `standard_user`<br>Password: `secret_sauce`     |

### Test Steps

1. Add a product to the shopping cart.
2. Click the shopping cart icon.
3. Verify that the added product appears in the cart.
4. Verify the product name and price.

### Expected Result

The product added to the cart should appear in the shopping cart with the correct product name and price.

### Actual Result

The added product appeared in the shopping cart. The product name and price were displayed.

### Status

**PASS**

## TC-012 — Add Multiple Products

| Field         | Details                                                  |
| ------------- | -------------------------------------------------------- |
| Test Case ID  | TC-012                                                   |
| Scenario ID   | TS-012                                                   |
| Title         | Verify that a user can add multiple products to the cart |
| Priority      | High                                                     |
| Preconditions | User is logged in and on the Products page               |
| Test Data     | Username: `standard_user`<br>Password: `secret_sauce`    |

### Test Steps

1. Add a product to the cart.
2. Add a second product to the cart.
3. Open the shopping cart.
4. Verify the number of products displayed.
5. Verify the cart count.

### Expected Result

Both selected products should appear in the shopping cart, and the cart count should display **2**.

### Actual Result

Two products were displayed in the shopping cart, and the cart count displayed **2**.

### Status

**PASS**

## TC-013 — Remove Product from Cart

| Field         | Details                                               |
| ------------- | ----------------------------------------------------- |
| Test Case ID  | TC-013                                                |
| Scenario ID   | TS-013                                                |
| Title         | Verify that a user can remove a product from the cart |
| Priority      | High                                                  |
| Preconditions | User is logged in and has two products in the cart    |
| Test Data     | Username: `standard_user`<br>Password: `secret_sauce` |

### Test Steps

1. Open the shopping cart containing two products.
2. Click the **Remove** button for one product.
3. Observe the products remaining in the cart.
4. Observe the cart count.

### Expected Result

The selected product should be removed from the cart. The remaining product should stay in the cart, and the cart count should decrease from 2 to 1.

### Actual Result

One product was removed successfully. One product remained in the cart, and the cart count changed to 1.

### Status

**PASS**

## TC-014 — Product Information in Cart

| Field         | Details                                                       |
| ------------- | ------------------------------------------------------------- |
| Test Case ID  | TC-014                                                        |
| Scenario ID   | TS-014                                                        |
| Title         | Verify that the cart displays the correct product information |
| Priority      | High                                                          |
| Preconditions | User is logged in and has a product in the shopping cart      |
| Test Data     | Username: `standard_user`<br>Password: `secret_sauce`         |

### Test Steps

1. Open the shopping cart.
2. Verify the product name.
3. Verify the product price.
4. Verify the product quantity.
5. Compare the displayed product information with the product originally selected.

### Expected Result

The cart should display the correct product name, price, and quantity. The displayed information should correspond to the product that was originally selected.

### Actual Result

The product name, price, and quantity were displayed, and the information corresponded to the product originally selected.

### Status

**PASS**

## TC-015 — Continue Shopping

| Field         | Details                                                         |
| ------------- | --------------------------------------------------------------- |
| Test Case ID  | TC-015                                                          |
| Scenario ID   | TS-015                                                          |
| Title         | Verify that a user can continue shopping after viewing the cart |
| Priority      | Medium                                                          |
| Preconditions | User is logged in and has a product in the shopping cart        |
| Test Data     | Username: `standard_user`<br>Password: `secret_sauce`           |

### Test Steps

1. Open the shopping cart.
2. Click the **Continue Shopping** button.
3. Observe the page displayed.
4. Verify that the previously added product remains in the cart.
5. Verify the cart count.

### Expected Result

The user should be returned to the Products page. The previously added product should remain in the cart, and the cart count should remain unchanged.

### Actual Result

After continuing shopping, the previously added product remained in the cart, and the cart count remained **1**.

### Status

**PASS**

## TC-016 — Proceed to Checkout

| Field         | Details                                                  |
| ------------- | -------------------------------------------------------- |
| Test Case ID  | TC-016                                                   |
| Scenario ID   | TS-016                                                   |
| Title         | Verify that a user can proceed from the cart to checkout |
| Priority      | High                                                     |
| Preconditions | User is logged in and has a product in the cart          |
| Test Data     | Username: `standard_user`<br>Password: `secret_sauce`    |

### Test Steps

1. Open the shopping cart.
2. Click the **Checkout** button.
3. Observe the checkout information page.
4. Verify that the First Name, Last Name, and Postal Code fields are displayed.
5. Verify that the **Continue** button is displayed.

### Expected Result

The user should be taken to the checkout information page, where the First Name, Last Name, Postal Code, and Continue button are available.

### Actual Result

The checkout information page opened successfully, and the First Name, Last Name, Postal Code, and Continue button were all available.

### Status

**PASS**

## TC-017 — Empty First Name

| Field         | Details                                                                               |
| ------------- | ------------------------------------------------------------------------------------- |
| Test Case ID  | TC-017                                                                                |
| Scenario ID   | TS-017                                                                                |
| Title         | Verify that checkout cannot proceed when the first name is empty                      |
| Priority      | High                                                                                  |
| Preconditions | User is logged in, has a product in the cart, and is on the checkout information page |
| Test Data     | First Name: *(empty)*<br>Last Name: `Mensah`<br>Postal Code: `Ge-159-0939`            |

### Test Steps

1. Leave the First Name field empty.
2. Enter `Mensah` in the Last Name field.
3. Enter `Ge-159-0939` in the Postal Code field.
4. Click **Continue**.

### Expected Result

The application should prevent the user from proceeding and display a validation message indicating that the First Name is required.

### Actual Result

The application prevented the user from proceeding and displayed the error message: **"First Name is required."**

### Status

**PASS**

## TC-018 — Empty Last Name

| Field         | Details                                                                               |
| ------------- | ------------------------------------------------------------------------------------- |
| Test Case ID  | TC-018                                                                                |
| Scenario ID   | TS-018                                                                                |
| Title         | Verify that checkout cannot proceed when the last name is empty                       |
| Priority      | High                                                                                  |
| Preconditions | User is logged in, has a product in the cart, and is on the checkout information page |
| Test Data     | First Name: Valid value<br>Last Name: *(empty)*<br>Postal Code: `Ge-159-0939`         |

### Test Steps

1. Enter a valid First Name.
2. Leave the Last Name field empty.
3. Enter `Ge-159-0939` in the Postal Code field.
4. Click **Continue**.

### Expected Result

The application should prevent the user from proceeding and display a validation message indicating that the Last Name is required.

### Actual Result

The application prevented the user from proceeding and displayed the error message: **"Last Name is required."**

### Status

**PASS**

## TC-019 — Empty Postal Code

| Field         | Details                                                                               |
| ------------- | ------------------------------------------------------------------------------------- |
| Test Case ID  | TC-019                                                                                |
| Scenario ID   | TS-019                                                                                |
| Title         | Verify that checkout cannot proceed when the postal code is empty                     |
| Priority      | High                                                                                  |
| Preconditions | User is logged in, has a product in the cart, and is on the checkout information page |
| Test Data     | First Name: Valid value<br>Last Name: `Mensah`<br>Postal Code: *(empty)*              |

### Test Steps

1. Enter a valid First Name.
2. Enter `Mensah` in the Last Name field.
3. Leave the Postal Code field empty.
4. Click **Continue**.

### Expected Result

The application should prevent the user from proceeding and display a validation message indicating that the Postal Code is required.

### Actual Result

The application prevented the user from proceeding and displayed the error message: **"Postal Code is required."**

### Status

**PASS**
## TC-020 — Complete Checkout with Valid Information

| Field | Details |
|---|---|
| Test Case ID | TC-020 |
| Scenario ID | TS-020 |
| Title | Verify that a user can proceed to checkout with valid customer information |
| Priority | High |
| Preconditions | User is logged in, has a product in the cart, and is on the checkout information page |
| Test Data | First Name: `Shadrack`<br>Last Name: `Mensah`<br>Postal Code: `GE-159-0939` |

### Test Steps

1. Enter `Shadrack` in the First Name field.
2. Enter `Mensah` in the Last Name field.
3. Enter `GE-159-0939` in the Postal Code field.
4. Click **Continue**.
5. Observe the page displayed.

### Expected Result

The application should accept the valid checkout information and navigate the user to the Checkout: Overview page.

### Actual Result

The application accepted the entered checkout information and navigated to the **Checkout: Overview** page.

### Status

**PASS**

## TC-021 — Verify Checkout Overview

| Field | Details |
|---|---|
| Test Case ID | TC-021 |
| Scenario ID | TS-021 |
| Title | Verify that the Checkout Overview page displays the correct order information |
| Priority | High |
| Preconditions | User has entered valid checkout information and is on the Checkout: Overview page |
| Test Data | Product: `Sauce Labs Backpack`<br>Quantity: `1`<br>Item Price: `$29.99` |

### Test Steps

1. Review the product displayed on the Checkout: Overview page.
2. Verify the quantity of the product.
3. Verify the product price.
4. Verify the Payment Information section.
5. Verify the Shipping Information section.
6. Verify the Item total.
7. Verify the Tax amount.
8. Verify the Total amount.
9. Verify that the **Cancel** and **Finish** buttons are displayed.

### Expected Result

The Checkout: Overview page should display the correct product, quantity, price, payment information, shipping information, item total, tax, total amount, and available **Cancel** and **Finish** buttons.

### Actual Result

The Checkout: Overview page displayed the **Sauce Labs Backpack** with quantity `1` and price `$29.99`. Payment Information displayed `SauceCard #31337`, Shipping Information displayed `Free Pony Express Delivery!`, Item total was `$29.99`, Tax was `$2.40`, and Total was `$32.39`. The **Cancel** and **Finish** buttons were also displayed.

### Status

**PASS**

## TC-022 — Verify Order Total

| Field | Details |
|---|---|
| Test Case ID | TC-022 |
| Scenario ID | TS-022 |
| Title | Verify that the checkout total is calculated correctly |
| Priority | High |
| Preconditions | User is on the Checkout: Overview page with a product in the order |
| Test Data | Item total: `$29.99`<br>Tax: `$2.40` |

### Test Steps

1. Note the Item total displayed on the Checkout: Overview page.
2. Note the Tax amount displayed.
3. Calculate the expected total by adding the Item total and Tax.
4. Compare the calculated amount with the Total displayed by the application.

### Expected Result

The Total should equal the Item total plus the Tax.

### Actual Result

The Item total was `$29.99` and the Tax was `$2.40`. The calculated total was `$32.39`, which matched the Total displayed by the application.

### Status

**PASS**

## TC-023 — Complete Order Successfully

| Field | Details |
|---|---|
| Test Case ID | TC-023 |
| Scenario ID | TS-023 |
| Title | Verify that a user can successfully complete an order |
| Priority | High |
| Preconditions | User is on the Checkout: Overview page with a valid order |
| Test Data | Sauce Labs Backpack, Quantity: `1`, Total: `$32.39` |

### Test Steps

1. Review the order details on the Checkout: Overview page.
2. Click **Finish**.
3. Observe the page displayed.

### Expected Result

The application should successfully process the order and navigate to the Checkout: Complete page displaying an order confirmation message.

### Actual Result

The application successfully processed the order and displayed the **Checkout: Complete!** page with the message **"Thank you for your order!"**. The page also displayed the order dispatch message and a **Back Home** button.

### Status

**PASS**

## TC-024 — Verify Order Confirmation

| Field | Details |
|---|---|
| Test Case ID | TC-024 |
| Scenario ID | TS-024 |
| Title | Verify that the order confirmation page displays the correct confirmation details |
| Priority | High |
| Preconditions | User has successfully completed an order and is on the Checkout: Complete page |
| Test Data | Completed order for Sauce Labs Backpack |

### Test Steps

1. Verify that the page displays **Checkout: Complete!**.
2. Verify that the page displays **Thank you for your order!**.
3. Verify that the order dispatch message is displayed.
4. Verify that the confirmation image is displayed.
5. Verify that the **Back Home** button is displayed.

### Expected Result

The Checkout: Complete page should clearly confirm that the order was successfully completed and provide an option to return to the Products page.

### Actual Result

The page displayed **Checkout: Complete!**, **Thank you for your order!**, the order dispatch message, the confirmation image, and the **Back Home** button.

### Status

**PASS**

## TC-025 — Return to Products After Order Completion

| Field | Details |
|---|---|
| Test Case ID | TC-025 |
| Scenario ID | TS-025 |
| Title | Verify that the user can return to the Products page after completing an order |
| Priority | Medium |
| Preconditions | User has successfully completed an order and is on the Checkout: Complete page |
| Test Data | Completed order for Sauce Labs Backpack |

### Test Steps

1. Click the **Back Home** button.
2. Observe the page displayed.

### Expected Result

The application should return the user to the Products page after completing the order.

### Actual Result

The application returned the user to the **Products** page after the **Back Home** button was clicked.

### Status

**PASS**