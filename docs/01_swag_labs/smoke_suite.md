# Smoke Suite — Swag Labs
**Tool:** testRigor | **App:** https://www.saucedemo.com | **Tests:** 8

---

### SM-01: Login page loads correctly
**Steps:**
1. check that page contains "Username"
2. check that page contains "Password"
3. check that page contains "Login"

**Expected:** Login page displays username, password fields and login button.

---

### SM-02: Valid login — standard user
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. check that page contains "Products"

**Expected:** Products inventory page is displayed after login.

---

### SM-03: Product inventory loads with items
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. check that page contains "Sauce Labs Backpack"

**Expected:** Product listing includes Sauce Labs Backpack.

---

### SM-04: Shopping cart icon visible on header
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. check that "shopping cart icon" is visible using ai

**Expected:** Shopping cart icon is visible in the header.

---

### SM-05: Add single item to cart
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Add to cart" below "Sauce Labs Backpack"
5. check that page contains "1"

**Expected:** Cart badge displays count 1 after adding item.

---

### SM-06: Navigation to cart page
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Add to cart" below "Sauce Labs Backpack"
5. scroll up
6. click "shopping cart icon" using ai
7. check that page contains "Your Cart"

**Expected:** Cart page displays with heading Your Cart.

---

### SM-07: Logout functionality
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Open Menu"
5. click "Logout"
6. check that page contains "Login"

**Expected:** User is redirected back to the login page after logout.

---

### SM-08: Continue shopping from cart
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Add to cart" below "Sauce Labs Backpack"
5. scroll up
6. click "shopping cart icon" using ai
7. check that page contains "Your Cart"
8. click "Continue Shopping"
9. check that page contains "Products"

**Expected:** User is taken back to the Products inventory page.
