# Test Cases – E-Commerce Web Application

## Project Information
- Application: SauceDemo (Swag Labs)
- Website: https://www.saucedemo.com/
- Testing Type: Manual Testing
- Testing Method: Black Box Testing
- Test Level: System Testing
- Test Environment: Web Browser
- Test Status: NOT RUN

## Objective
To verify that the main features of the e-commerce application work as expected, including login, inventory, product sorting, shopping cart, checkout, and order completion.

---

# 1. Login Test Cases

## TC-LOGIN-001 – Login with Valid Credentials

| Field | Description |
|---|---|
| Test Case ID | TC-LOGIN-001 |
| Scenario ID | TS-LOGIN-001 |
| Module | Login |
| Test Type | Positive |
| Priority | High |

### Preconditions
- User is on the login page.
- User account is active.

### Test Data
- Username: standard_user
- Password: secret_sauce

### Test Steps
1. Open https://www.saucedemo.com/
2. Enter a valid username.
3. Enter a valid password.
4. Click the Login button.

### Expected Result
- User successfully logs in.
- User is redirected to the inventory page.
- Available products are displayed.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-LOGIN-002 – Login with Invalid Password

| Field | Description |
|---|---|
| Test Case ID | TC-LOGIN-002 |
| Scenario ID | TS-LOGIN-002 |
| Module | Login |
| Test Type | Negative |
| Priority | High |

### Preconditions
- User is on the login page.

### Test Data
- Username: standard_user
- Password: invalid_password

### Test Steps
1. Open the login page.
2. Enter a valid username.
3. Enter an invalid password.
4. Click the Login button.

### Expected Result
- Login is rejected.
- User remains on the login page.
- An appropriate error message is displayed.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-LOGIN-003 – Login with Invalid Username

| Field | Description |
|---|---|
| Test Case ID | TC-LOGIN-003 |
| Scenario ID | TS-LOGIN-003 |
| Module | Login |
| Test Type | Negative |
| Priority | High |

### Preconditions
- User is on the login page.

### Test Data
- Username: invalid_user
- Password: secret_sauce

### Test Steps
1. Open the login page.
2. Enter an invalid username.
3. Enter a valid password.
4. Click the Login button.

### Expected Result
- Login is rejected.
- User remains on the login page.
- An appropriate error message is displayed.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-LOGIN-004 – Login with Empty Username

| Field | Description |
|---|---|
| Test Case ID | TC-LOGIN-004 |
| Scenario ID | TS-LOGIN-004 |
| Module | Login |
| Test Type | Negative |
| Priority | High |

### Preconditions
- User is on the login page.

### Test Data
- Username: Empty
- Password: secret_sauce

### Test Steps
1. Open the login page.
2. Leave the username field empty.
3. Enter a valid password.
4. Click the Login button.

### Expected Result
- Login is rejected.
- User remains on the login page.
- A validation error related to the username is displayed.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-LOGIN-005 – Login with Empty Password

| Field | Description |
|---|---|
| Test Case ID | TC-LOGIN-005 |
| Scenario ID | TS-LOGIN-005 |
| Module | Login |
| Test Type | Negative |
| Priority | High |

### Preconditions
- User is on the login page.

### Test Data
- Username: standard_user
- Password: Empty

### Test Steps
1. Open the login page.
2. Enter a valid username.
3. Leave the password field empty.
4. Click the Login button.

### Expected Result
- Login is rejected.
- User remains on the login page.
- A validation error related to the password is displayed.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-LOGIN-006 – Login with Locked User

| Field | Description |
|---|---|
| Test Case ID | TC-LOGIN-006 |
| Scenario ID | TS-LOGIN-006 |
| Module | Login |
| Test Type | Negative |
| Priority | High |

### Preconditions
- User is on the login page.

### Test Data
- Username: locked_out_user
- Password: secret_sauce

### Test Steps
1. Open the login page.
2. Enter the locked user account.
3. Enter the correct password.
4. Click the Login button.

### Expected Result
- Login is rejected.
- User is not redirected to the inventory page.
- An appropriate locked-account error message is displayed.

### Actual Result
Not executed.

### Status
NOT RUN

---

# 2. Inventory Test Cases

## TC-INV-001 – Verify Inventory Page After Login

| Field | Description |
|---|---|
| Test Case ID | TC-INV-001 |
| Scenario ID | TS-INV-001 |
| Module | Inventory |
| Test Type | Positive |
| Priority | High |

### Preconditions
- User has valid credentials.

### Test Data
- Username: standard_user
- Password: secret_sauce

### Test Steps
1. Open the login page.
2. Login using valid credentials.
3. Observe the inventory page.

### Expected Result
- User is redirected to the inventory page.
- Inventory page is displayed successfully.
- Product list is visible.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-INV-002 – Verify All Available Products Are Displayed

| Field | Description |
|---|---|
| Test Case ID | TC-INV-002 |
| Scenario ID | TS-INV-002 |
| Module | Inventory |
| Test Type | Positive |
| Priority | High |

### Preconditions
- User is logged in.
- Inventory page is displayed.

### Test Data
- Valid user account.

### Test Steps
1. Login to the application.
2. Open the inventory page.
3. Observe the available products.
4. Verify the product list against the application data.

### Expected Result
- All expected products are displayed.
- No product is missing from the inventory list.
- No unexpected duplicate product is displayed.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-INV-003 – Verify Product Names and Prices

| Field | Description |
|---|---|
| Test Case ID | TC-INV-003 |
| Scenario ID | TS-INV-003 |
| Module | Inventory |
| Test Type | Positive |
| Priority | High |

### Preconditions
- User is logged in.
- Inventory page is displayed.

### Test Data
- All products available in the inventory.

### Test Steps
1. Login to the application.
2. Open the inventory page.
3. Check each product name.
4. Check each product price.
5. Compare the displayed information with the expected product data.

### Expected Result
- Product names are correct.
- Product prices are correct.
- Each price is associated with the correct product.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-INV-004 – Verify Product Images

| Field | Description |
|---|---|
| Test Case ID | TC-INV-004 |
| Scenario ID | TS-INV-004 |
| Module | Inventory |
| Test Type | Positive |
| Priority | Medium |

### Preconditions
- User is logged in.
- Inventory page is displayed.

### Test Data
- All products available in the inventory.

### Test Steps
1. Login to the application.
2. Open the inventory page.
3. Observe all product images.
4. Verify that each image matches its corresponding product.

### Expected Result
- Product images are displayed successfully.
- Images are not broken or missing.
- Each image represents the correct product.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-INV-005 – Verify Product Detail Page

| Field | Description |
|---|---|
| Test Case ID | TC-INV-005 |
| Scenario ID | TS-INV-005 |
| Module | Inventory |
| Test Type | Positive |
| Priority | Medium |

### Preconditions
- User is logged in.
- Inventory page is displayed.

### Test Data
- Sauce Labs Backpack.

### Test Steps
1. Login to the application.
2. Open the inventory page.
3. Select Sauce Labs Backpack.
4. Observe the product detail page.
5. Verify the product name, price, image, and description.

### Expected Result
- The selected product detail page is displayed.
- Product name matches the selected item.
- Product price matches the inventory price.
- Product image and description are displayed correctly.

### Actual Result
Not executed.

### Status
NOT RUN

---

# 3. Sorting Test Cases

## TC-SORT-001 – Sort Products by Name A to Z

| Field | Description |
|---|---|
| Test Case ID | TC-SORT-001 |
| Scenario ID | TS-SORT-001 |
| Module | Sorting |
| Test Type | Positive |
| Priority | Medium |

### Preconditions
- User is logged in.
- Inventory page is displayed.

### Test Data
- Sort option: Name (A to Z)

### Test Steps
1. Login to the application.
2. Open the inventory page.
3. Click the sorting dropdown.
4. Select Name (A to Z).
5. Observe the product order.

### Expected Result
- Products are sorted alphabetically from A to Z.
- The product order is correct.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-SORT-002 – Sort Products by Name Z to A

| Field | Description |
|---|---|
| Test Case ID | TC-SORT-002 |
| Scenario ID | TS-SORT-002 |
| Module | Sorting |
| Test Type | Positive |
| Priority | Medium |

### Preconditions
- User is logged in.
- Inventory page is displayed.

### Test Data
- Sort option: Name (Z to A)

### Test Steps
1. Login to the application.
2. Open the inventory page.
3. Click the sorting dropdown.
4. Select Name (Z to A).
5. Observe the product order.

### Expected Result
- Products are sorted alphabetically from Z to A.
- The product order is correct.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-SORT-003 – Sort Products by Price Low to High

| Field | Description |
|---|---|
| Test Case ID | TC-SORT-003 |
| Scenario ID | TS-SORT-003 |
| Module | Sorting |
| Test Type | Positive |
| Priority | High |

### Preconditions
- User is logged in.
- Inventory page is displayed.

### Test Data
- Sort option: Price (low to high)

### Test Steps
1. Login to the application.
2. Open the inventory page.
3. Click the sorting dropdown.
4. Select Price (low to high).
5. Observe the product prices.

### Expected Result
- Products are sorted from the lowest price to the highest price.
- The product order matches the ascending price order.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-SORT-004 – Sort Products by Price High to Low

| Field | Description |
|---|---|
| Test Case ID | TC-SORT-004 |
| Scenario ID | TS-SORT-004 |
| Module | Sorting |
| Test Type | Positive |
| Priority | High |

### Preconditions
- User is logged in.
- Inventory page is displayed.

### Test Data
- Sort option: Price (high to low)

### Test Steps
1. Login to the application.
2. Open the inventory page.
3. Click the sorting dropdown.
4. Select Price (high to low).
5. Observe the product prices.

### Expected Result
- Products are sorted from the highest price to the lowest price.
- The product order matches the descending price order.

### Actual Result
Not executed.

### Status
NOT RUN

---

# 4. Shopping Cart Test Cases

## TC-CART-001 – Add One Product to Shopping Cart

| Field | Description |
|---|---|
| Test Case ID | TC-CART-001 |
| Scenario ID | TS-CART-001 |
| Module | Shopping Cart |
| Test Type | Positive |
| Priority | High |

### Preconditions
- User is logged in.
- Inventory page is displayed.
- Shopping cart is empty.

### Test Data
- Product: Sauce Labs Backpack

### Test Steps
1. Login to the application.
2. Select Sauce Labs Backpack.
3. Click Add to cart.
4. Observe the shopping cart badge.
5. Open the shopping cart.

### Expected Result
- Product is added to the cart successfully.
- Cart badge displays 1.
- The selected product is displayed in the cart.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-CART-002 – Add Multiple Products to Shopping Cart

| Field | Description |
|---|---|
| Test Case ID | TC-CART-002 |
| Scenario ID | TS-CART-002 |
| Module | Shopping Cart |
| Test Type | Positive |
| Priority | High |

### Preconditions
- User is logged in.
- Inventory page is displayed.
- Shopping cart is empty.

### Test Data
- Sauce Labs Backpack
- Sauce Labs Bike Light

### Test Steps
1. Login to the application.
2. Click Add to cart for Sauce Labs Backpack.
3. Click Add to cart for Sauce Labs Bike Light.
4. Observe the shopping cart badge.
5. Open the shopping cart.

### Expected Result
- Both products are added successfully.
- Cart badge displays 2.
- Both products are displayed in the shopping cart.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-CART-003 – Remove Selected Product from Shopping Cart

| Field | Description |
|---|---|
| Test Case ID | TC-CART-003 |
| Scenario ID | TS-CART-003 |
| Module | Shopping Cart |
| Test Type | Positive |
| Priority | High |

### Preconditions
- User is logged in.
- Two products are already added to the cart.

### Test Data
- Sauce Labs Backpack
- Sauce Labs Bike Light

### Test Steps
1. Login to the application.
2. Add Sauce Labs Backpack to the cart.
3. Add Sauce Labs Bike Light to the cart.
4. Open the shopping cart.
5. Click Remove for Sauce Labs Backpack.

### Expected Result
- Sauce Labs Backpack is removed.
- Sauce Labs Bike Light remains in the cart.
- Cart badge reflects the remaining product count.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-CART-004 – Verify Shopping Cart Item Count

| Field | Description |
|---|---|
| Test Case ID | TC-CART-004 |
| Scenario ID | TS-CART-004 |
| Module | Shopping Cart |
| Test Type | Validation |
| Priority | Medium |

### Preconditions
- User is logged in.
- Inventory page is displayed.

### Test Data
- Sauce Labs Backpack
- Sauce Labs Bike Light
- Sauce Labs Bolt T-Shirt

### Test Steps
1. Login to the application.
2. Add Sauce Labs Backpack to the cart.
3. Add Sauce Labs Bike Light to the cart.
4. Add Sauce Labs Bolt T-Shirt to the cart.
5. Verify the cart badge.
6. Remove one product.
7. Verify the cart badge again.

### Expected Result
- Cart badge displays 3 after adding three products.
- Cart badge displays 2 after removing one product.
- Cart badge count matches the number of items in the cart.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-CART-005 – Verify Shopping Cart Product Data

| Field | Description |
|---|---|
| Test Case ID | TC-CART-005 |
| Scenario ID | TS-CART-005 |
| Module | Shopping Cart |
| Test Type | Positive |
| Priority | High |

### Preconditions
- User is logged in.
- Products have been added to the cart.

### Test Data
- Sauce Labs Backpack
- Sauce Labs Bike Light

### Test Steps
1. Login to the application.
2. Add Sauce Labs Backpack to the cart.
3. Add Sauce Labs Bike Light to the cart.
4. Open the shopping cart.
5. Verify each product name.
6. Verify each product price.
7. Verify the product quantity.

### Expected Result
- All selected products are displayed.
- Product names match the selected products.
- Product prices match the inventory prices.
- Product quantities are correct.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-CART-006 – Verify Shopping Cart When All Products Are Removed

| Field | Description |
|---|---|
| Test Case ID | TC-CART-006 |
| Scenario ID | TS-CART-006 |
| Module | Shopping Cart |
| Test Type | Edge Case |
| Priority | Medium |

### Preconditions
- User is logged in.
- At least one product is added to the cart.

### Test Data
- Sauce Labs Backpack
- Sauce Labs Bike Light

### Test Steps
1. Login to the application.
2. Add Sauce Labs Backpack to the cart.
3. Add Sauce Labs Bike Light to the cart.
4. Open the shopping cart.
5. Remove Sauce Labs Backpack.
6. Remove Sauce Labs Bike Light.
7. Observe the shopping cart.

### Expected Result
- All products are removed successfully.
- Shopping cart displays no products.
- Cart badge is no longer displayed or reflects an empty cart according to the application behavior.

### Actual Result
Not executed.

### Status
NOT RUN

---

# 5. Checkout Test Cases

## TC-CHK-001 – Checkout with Valid Customer Information

| Field | Description |
|---|---|
| Test Case ID | TC-CHK-001 |
| Scenario ID | TS-CHK-001 |
| Module | Checkout |
| Test Type | Positive |
| Priority | High |

### Preconditions
- User is logged in.
- At least one product is added to the cart.

### Test Data
- First Name: Budi
- Last Name: Santoso
- Zip/Postal Code: 15157

### Test Steps
1. Login to the application.
2. Add Sauce Labs Backpack to the cart.
3. Open the shopping cart.
4. Click Checkout.
5. Enter First Name.
6. Enter Last Name.
7. Enter Zip/Postal Code.
8. Click Continue.

### Expected Result
- Customer information is accepted.
- User is redirected to the Checkout Overview page.
- Order details are displayed.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-CHK-002 – Checkout with Empty First Name

| Field | Description |
|---|---|
| Test Case ID | TC-CHK-002 |
| Scenario ID | TS-CHK-002 |
| Module | Checkout |
| Test Type | Negative |
| Priority | High |

### Preconditions
- User is logged in.
- At least one product is added to the cart.
- User is on the Checkout Information page.

### Test Data
- First Name: Empty
- Last Name: Santoso
- Zip/Postal Code: 15157

### Test Steps
1. Open the shopping cart.
2. Click Checkout.
3. Leave First Name empty.
4. Enter Last Name.
5. Enter Zip/Postal Code.
6. Click Continue.

### Expected Result
- Checkout process is rejected.
- User remains on the Checkout Information page.
- Validation error for First Name is displayed.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-CHK-003 – Checkout with Empty Last Name

| Field | Description |
|---|---|
| Test Case ID | TC-CHK-003 |
| Scenario ID | TS-CHK-003 |
| Module | Checkout |
| Test Type | Negative |
| Priority | High |

### Preconditions
- User is logged in.
- At least one product is added to the cart.
- User is on the Checkout Information page.

### Test Data
- First Name: Budi
- Last Name: Empty
- Zip/Postal Code: 15157

### Test Steps
1. Open the shopping cart.
2. Click Checkout.
3. Enter First Name.
4. Leave Last Name empty.
5. Enter Zip/Postal Code.
6. Click Continue.

### Expected Result
- Checkout process is rejected.
- User remains on the Checkout Information page.
- Validation error for Last Name is displayed.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-CHK-004 – Checkout with Empty Postal Code

| Field | Description |
|---|---|
| Test Case ID | TC-CHK-004 |
| Scenario ID | TS-CHK-004 |
| Module | Checkout |
| Test Type | Negative |
| Priority | High |

### Preconditions
- User is logged in.
- At least one product is added to the cart.
- User is on the Checkout Information page.

### Test Data
- First Name: Budi
- Last Name: Santoso
- Zip/Postal Code: Empty

### Test Steps
1. Open the shopping cart.
2. Click Checkout.
3. Enter First Name.
4. Enter Last Name.
5. Leave Zip/Postal Code empty.
6. Click Continue.

### Expected Result
- Checkout process is rejected.
- User remains on the Checkout Information page.
- Validation error for Postal Code is displayed.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-CHK-005 – Verify Checkout Order Summary and Price Calculation

| Field | Description |
|---|---|
| Test Case ID | TC-CHK-005 |
| Scenario ID | TS-CHK-005 |
| Module | Checkout |
| Test Type | Validation |
| Priority | High |

### Preconditions
- User is logged in.
- Products have been added to the shopping cart.
- User has entered valid checkout information.

### Test Data
- Sauce Labs Backpack: $29.99
- Sauce Labs Bike Light: $9.99
- Expected Subtotal: $39.98
- Tax: Calculated by the application
- Total: Subtotal + Tax

### Test Steps
1. Login to the application.
2. Add Sauce Labs Backpack to the cart.
3. Add Sauce Labs Bike Light to the cart.
4. Open the shopping cart.
5. Click Checkout.
6. Enter valid customer information.
7. Click Continue.
8. Verify product names.
9. Verify individual product prices.
10. Verify subtotal.
11. Verify tax.
12. Verify total price.

### Expected Result
- Product names match the selected products.
- Product prices are correct.
- Subtotal equals the sum of all product prices.
- Tax is calculated correctly according to the application.
- Total equals subtotal plus tax.

### Actual Result
Not executed.

### Status
NOT RUN

---

# 6. Order Completion Test Cases

## TC-ORD-001 – Complete Order Successfully

| Field | Description |
|---|---|
| Test Case ID | TC-ORD-001 |
| Scenario ID | TS-ORD-001 |
| Module | Order Completion |
| Test Type | Positive |
| Priority | High |

### Preconditions
- User is logged in.
- At least one product is added to the cart.
- Customer checkout information has been entered.
- Checkout Overview page is displayed.

### Test Data
- Sauce Labs Backpack
- Valid customer information

### Test Steps
1. Login to the application.
2. Add a product to the cart.
3. Open the shopping cart.
4. Click Checkout.
5. Enter valid customer information.
6. Click Continue.
7. Review the order.
8. Click Finish.

### Expected Result
- Order is completed successfully.
- User is redirected to the order confirmation page.
- Order completion message is displayed.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-ORD-002 – Verify Order Confirmation Message

| Field | Description |
|---|---|
| Test Case ID | TC-ORD-002 |
| Scenario ID | TS-ORD-002 |
| Module | Order Completion |
| Test Type | Validation |
| Priority | High |

### Preconditions
- User has completed the checkout process.
- Order confirmation page is displayed.

### Test Data
- Completed order.

### Test Steps
1. Complete a purchase using valid checkout information.
2. Click Finish on the Checkout Overview page.
3. Observe the order confirmation page.
4. Verify the confirmation message.

### Expected Result
- Order confirmation page is displayed.
- Confirmation message is visible.
- Message indicates that the order has been completed successfully.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-ORD-003 – Return to Inventory Using Back Home

| Field | Description |
|---|---|
| Test Case ID | TC-ORD-003 |
| Scenario ID | TS-ORD-003 |
| Module | Order Completion |
| Test Type | Positive |
| Priority | Medium |

### Preconditions
- User has successfully completed an order.
- Order confirmation page is displayed.

### Test Data
- Completed order.

### Test Steps
1. Complete the checkout process.
2. Verify the order confirmation page.
3. Click Back Home.
4. Observe the destination page.

### Expected Result
- User is redirected to the inventory page.
- Inventory products are displayed.
- User can continue browsing products.

### Actual Result
Not executed.

### Status
NOT RUN

---

## TC-ORD-004 – Verify Shopping Cart Is Empty After Order Completion

| Field | Description |
|---|---|
| Test Case ID | TC-ORD-004 |
| Scenario ID | TS-ORD-004 |
| Module | Order Completion |
| Test Type | Data Consistency |
| Priority | High |

### Preconditions
- User is logged in.
- At least one product has been purchased successfully.
- User has returned to the inventory page.

### Test Data
- Sauce Labs Backpack

### Test Steps
1. Login to the application.
2. Add Sauce Labs Backpack to the cart.
3. Complete the checkout process.
4. Click Finish.
5. Click Back Home.
6. Observe the shopping cart badge.
7. Open the shopping cart.

### Expected Result
- Previous purchased products are no longer present in the shopping cart.
- Shopping cart is empty after successful order completion.
- Cart state is consistent with the completed order.

### Actual Result
Not executed.

### Status
NOT RUN

---

# 7. Test Execution Summary

| Metric | Result |
|---|---|
| Total Test Cases | 30 |
| Executed | 0 |
| Passed | 0 |
| Failed | 0 |
| Blocked | 0 |
| Not Run | 30 |
| Pass Rate | N/A |

## Test Execution Notes
- Test cases have been designed but not executed.
- Actual results will be updated during manual testing.
- PASS or FAIL status will be assigned based on the observed application behavior.
- Screenshots will be collected as test evidence.
- Failed test cases will be documented in the Bug Reports folder.

---

# 8. Test Case Status Legend

| Status | Description |
|---|---|
| PASS | Actual result matches expected result |
| FAIL | Actual result does not match expected result |
| BLOCKED | Test execution cannot continue due to an issue |
| NOT RUN | Test case has not been executed |

---

# 9. Test Conclusion

A total of 30 test cases have been prepared to validate the main functionality of the SauceDemo e-commerce application.

The test cases cover login, inventory, sorting, shopping cart, checkout, and order completion.

Test execution is pending. The final testing conclusion will be determined after all test cases have been executed and the results have been documented.
