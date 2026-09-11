# Exploratory Testing Session

## Session Information

**Application:** SauceDemo / Swag Labs

**Application URL:** https://www.saucedemo.com/

**Session Duration:** 45 minutes

**Testing Approach:** Exploratory Testing

**Primary Environment:** Chrome on macOS (MacBook)

**Tester:** Shadrack Mensah

## Session Objective

The purpose of this exploratory session was to investigate the application's navigation, state management, checkout behavior, browser navigation, logout behavior, and recovery from common user actions beyond the planned test cases.

## Areas Explored

- Application menu and navigation
- Logout behavior
- Browser Back navigation
- Browser Refresh behavior
- Cart state and cart badge
- Reset App State
- Checkout information persistence
- Checkout navigation
- Repeated Add to Cart interaction
- Order completion flow

## Exploratory Findings

### 1. Application Menu

The application menu was opened from the Products page. The available navigation options included All Items, About, Logout, and Reset App State.

**Observation:** The menu provided access to the main navigation and application-state actions.

### 2. Logout Behavior

Logout was selected from the application menu.

**Result:** The application returned to the login page.

The browser Back button was then used after logout.

**Result:** The login page remained displayed and the previously authenticated Products page was not restored.

**Assessment:** No confirmed defect observed.

### 3. Reset App State

A product was added to the cart and Reset App State was selected from the menu.

**Result:** The cart became empty.

**Assessment:** The reset function worked as expected. The action may benefit from clear user feedback because it removes the current application state.

### 4. Cart Persistence After Browser Refresh

A product was added to the cart and the browser was refreshed.

**Result:** The product remained in the cart after the refresh.

**Assessment:** Cart state persisted as expected.

### 5. Checkout Overview After Browser Refresh

The checkout process was completed up to the Checkout: Overview page. The browser was refreshed.

**Result:** The Checkout Overview and order information remained intact.

**Assessment:** No unexpected loss of checkout information was observed.

### 6. Browser Back During Checkout

From the Checkout: Overview page, the browser Back button was selected.

**Result:** The application returned to the Checkout: Your Information page.

**Assessment:** The behavior was recorded as a navigation observation. No confirmed defect was identified.

### 7. Repeated Add to Cart Interaction

A product was added to the cart.

**Result:** The Add to cart button changed to Remove, preventing another Add to cart action on the same product.

**Assessment:** No duplicate-add behavior was observed during the check.

### 8. Cart Badge After Removing an Item

Multiple products were added to the cart and one item was removed.

**Result:** The cart count decreased accordingly.

**Assessment:** Cart badge behavior worked as expected.

## Questions and Risks Identified

- Is the browser-back behavior during checkout consistent with the intended user journey?
- Should Reset App State provide additional confirmation or feedback before clearing application state?
- Should the application provide stronger visual feedback when important navigation or state-changing actions occur?

## Overall Session Assessment

The exploratory checks did not identify a confirmed functional defect. The main observations were related to navigation behavior and application-state management.

The exploratory session provided additional coverage beyond the planned test cases, particularly around browser navigation, refresh behavior, logout, cart persistence, and application-state reset.
