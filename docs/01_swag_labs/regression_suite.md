# Regression Suite — Swag Labs
**Tool:** testRigor | **App:** https://www.saucedemo.com | **Tests:** 20

---

### REG-01: Complete checkout — single item
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Add to cart" below "Sauce Labs Backpack"
5. scroll up
6. click "shopping cart icon" using ai
7. check that page contains "Sauce Labs Backpack"
8. click "Checkout"
9. enter "Vamshi" into "First Name"
10. enter "Reddy" into "Last Name"
11. enter "500001" into "Zip/Postal Code"
12. click "Continue"
13. check that page contains "Payment Information"
14. click "Finish"
15. check that page contains "Thank you for your order!"

**Expected:** Order confirmation page with Thank you for your order! message.

---

### REG-02: Complete checkout — multiple items
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Add to cart" below "Sauce Labs Backpack"
5. click "Add to cart" below "Sauce Labs Bike Light"
6. scroll up
7. click "shopping cart icon" using ai
8. check that page contains "Sauce Labs Backpack"
9. check that page contains "Sauce Labs Bike Light"
10. click "Checkout"
11. enter "Vamshi" into "First Name"
12. enter "Reddy" into "Last Name"
13. enter "500001" into "Zip/Postal Code"
14. click "Continue"
15. click "Finish"
16. check that page contains "Thank you for your order!"

**Expected:** Both items appear in cart; order confirmation shown.

---

### REG-03: Product price displayed correctly
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. check that page contains "$29.99"

**Expected:** Price $29.99 (Backpack) is visible on product listing.

---

### REG-04: Product detail page navigation
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Sauce Labs Backpack"
5. check that page contains "carry.allTheThings()"

**Expected:** Product description text is visible on the detail page.

---

### REG-05: Add to cart from product detail page
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Sauce Labs Backpack"
5. click "Add to cart"
6. check that page contains "1"

**Expected:** Cart badge shows 1 after adding from detail page.

---

### REG-06: Remove item from cart
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Add to cart" below "Sauce Labs Backpack"
5. scroll up
6. click "shopping cart icon" using ai
7. check that page contains "Sauce Labs Backpack"
8. click "Remove" using ai
9. check that page contains "Your Cart"
10. check that page doesn't contain "Sauce Labs Backpack"

**Expected:** Cart page remains but item name no longer appears after removal.

---

### REG-07: Sort products — Name A to Z
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. select "Name (A to Z)" from "Name (A to Z)"
5. check that page contains "Sauce Labs Backpack"

**Expected:** Products are displayed in A-Z alphabetical order.

---

### REG-08: Sort products — Name Z to A
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. select "Name (Z to A)" from "Name (A to Z)"
5. check that page contains "Sauce Labs Onesie"

**Expected:** Last product alphabetically appears first in listing.

---

### REG-09: Sort products — Price low to high
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. select "Price (low to high)" from "Name (A to Z)"
5. check that page contains "$7.99"

**Expected:** Lowest priced product $7.99 appears at top.

---

### REG-10: Sort products — Price high to low
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. select "Price (high to low)" from "Name (A to Z)"
5. check that page contains "$49.99"

**Expected:** Most expensive product $49.99 Fleece Jacket appears first.

---

### REG-11: Cart persists across navigation
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Add to cart" below "Sauce Labs Backpack"
5. click "Sauce Labs Bike Light"
6. click "Back to products"
7. check that page contains "1"

**Expected:** Cart badge still shows 1 after navigating away and back.

---

### REG-12: Checkout overview shows item details
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Add to cart" below "Sauce Labs Backpack"
5. scroll up
6. click "shopping cart icon" using ai
7. click "Checkout"
8. enter "Vamshi" into "First Name"
9. enter "Reddy" into "Last Name"
10. enter "500001" into "Zip/Postal Code"
11. click "Continue"
12. check that page contains "Sauce Labs Backpack"
13. check that page contains "$29.99"

**Expected:** Checkout overview shows item name and correct price.

---

### REG-13: Tax is applied at checkout
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Add to cart" below "Sauce Labs Backpack"
5. scroll up
6. click "shopping cart icon" using ai
7. click "Checkout"
8. enter "Vamshi" into "First Name"
9. enter "Reddy" into "Last Name"
10. enter "500001" into "Zip/Postal Code"
11. click "Continue"
12. check that page contains "Tax:"

**Expected:** Tax line item is visible in the order summary.

---

### REG-14: Cancel checkout returns to cart
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Add to cart" below "Sauce Labs Backpack"
5. scroll up
6. click "shopping cart icon" using ai
7. click "Checkout"
8. click "Cancel"
9. check that page contains "Your Cart"

**Expected:** User is returned to the cart page after cancelling checkout.

---

### REG-15: Cancel on overview returns to products
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Add to cart" below "Sauce Labs Backpack"
5. scroll up
6. click "shopping cart icon" using ai
7. click "Checkout"
8. enter "Vamshi" into "First Name"
9. enter "Reddy" into "Last Name"
10. enter "500001" into "Zip/Postal Code"
11. click "Continue"
12. click "Cancel"
13. check that page contains "Products"

**Expected:** User is taken back to the Products page on Cancel from overview.

---

### REG-16: All 6 products visible on inventory
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. check that page contains "Sauce Labs Backpack"
5. check that page contains "Sauce Labs Bike Light"
6. check that page contains "Sauce Labs Bolt T-Shirt"
7. check that page contains "Sauce Labs Fleece Jacket"
8. check that page contains "Sauce Labs Onesie"
9. check that page contains "Test.allTheThings() T-Shirt"

**Expected:** All six products are displayed on the inventory page.

---

### REG-17: Remove item directly from inventory
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Add to cart" below "Sauce Labs Bike Light"
5. check that page contains "Remove"
6. click "Remove" below "Sauce Labs Bike Light"
7. check that page contains "Add to cart" below "Sauce Labs Bike Light"

**Expected:** Remove button disappears; Add to cart button returns on inventory page.

---

### REG-18: Hamburger menu items visible
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Open Menu"
5. check that page contains "All Items"
6. check that page contains "About"
7. check that page contains "Logout"
8. check that page contains "Reset App State"

**Expected:** All four menu items are visible in the hamburger nav.

---

### REG-19: Reset app state clears cart
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Add to cart" below "Sauce Labs Backpack"
5. check that page contains "1"
6. click "Open Menu"
7. click "Reset App State"
8. scroll up
9. click "shopping cart icon" using ai
10. check that page doesn't contain "Sauce Labs Backpack"

**Expected:** Cart is empty after Reset App State.

---

### REG-20: Order confirmation — back home button
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Add to cart" below "Sauce Labs Backpack"
5. scroll up
6. click "shopping cart icon" using ai
7. click "Checkout"
8. enter "Vamshi" into "First Name"
9. enter "Reddy" into "Last Name"
10. enter "500001" into "Zip/Postal Code"
11. click "Continue"
12. click "Finish"
13. check that page contains "Thank you for your order!"
14. click "Back Home"
15. check that page contains "Products"

**Expected:** Clicking Back Home after order returns user to product listing.
