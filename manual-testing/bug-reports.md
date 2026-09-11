# Bug Reports and Quality Observations

## Observation 1 — Browser Back During Checkout

**Type:** Quality Observation

**Area:** Checkout Navigation

**Severity:** Low

**Environment:** Chrome on macOS (MacBook)

**Steps to Reproduce:**
1. Log in with valid credentials.
2. Add a product to the cart.
3. Proceed to checkout.
4. Complete the required customer information.
5. Reach the Checkout: Overview page.
6. Click the browser Back button.

**Expected Result:**
The application should provide a clear and predictable navigation experience when the user moves backward from the checkout flow.

**Actual Result:**
The browser Back button returned the user from the Checkout: Overview page to the Checkout: Your Information page.

**Assessment:**
No functional defect was confirmed. The behavior was observed during exploratory testing and is recorded as a navigation observation because users may need to understand whether previously entered checkout information is retained when navigating backward.

**Status:** Observation — No confirmed defect

## Observation 2 — Browser Back After Logout

**Type:** Quality Observation

**Area:** Logout and Session Navigation

**Severity:** Low

**Environment:** Chrome on macOS (MacBook)

**Steps to Reproduce:**
1. Log in with valid credentials.
2. Navigate to the Products page.
3. Select Logout from the menu.
4. After returning to the login page, click the browser Back button.

**Expected Result:**
After logout, using the browser Back button should not provide access to the previously authenticated Products page.

**Actual Result:**
After logout, clicking the browser Back button did not restore the Products page. The login page remained displayed.

**Assessment:**
No security defect was confirmed. The observed behavior indicates that the application does not expose the previously authenticated Products page through browser Back after logout.

**Status:** Observation — No confirmed defect

## Observation 3 — Reset App State Clears Cart Data

**Type:** Quality Observation

**Area:** Application State Management

**Severity:** Low

**Environment:** Chrome on macOS (MacBook)

**Steps to Reproduce:**
1. Log in with valid credentials.
2. Add a product to the cart.
3. Open the application menu.
4. Select **Reset App State**.
5. Open the cart.

**Expected Result:**
The application should clearly communicate that resetting the application state will remove the current cart state.

**Actual Result:**
After selecting **Reset App State**, the cart became empty.

**Assessment:**
The reset behavior worked as expected. No functional defect was confirmed. The observation is recorded because clearing application state is a significant action and clear user feedback or confirmation could help prevent accidental loss of cart information.

**Status:** Observation — No confirmed defect
