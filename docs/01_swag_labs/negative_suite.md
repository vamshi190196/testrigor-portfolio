# Negative Suite — Swag Labs
**Tool:** testRigor | **App:** https://www.saucedemo.com | **Tests:** 10

---

### NEG-01: Login with locked out user
**Steps:**
1. enter "locked_out_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. check that page contains "Sorry, this user has been locked out."

**Expected:** Error: Sorry, this user has been locked out.

---

### NEG-02: Login with incorrect password
**Steps:**
1. enter "standard_user" into "Username"
2. enter "wrongpassword" into "Password"
3. click "Login"
4. check that page contains "Username and password do not match"

**Expected:** Error: Username and password do not match any user in this service.

---

### NEG-03: Login with empty username
**Steps:**
1. click "Login"
2. check that page contains "Username is required"

**Expected:** Error: Epic sadface: Username is required.

---

### NEG-04: Login with empty password
**Steps:**
1. enter "standard_user" into "Username"
2. click "Login"
3. check that page contains "Password is required"

**Expected:** Error: Epic sadface: Password is required.

---

### NEG-05: Login with non-existent username
**Steps:**
1. enter "unknownuser123" into "Username"
2. enter "anypassword" into "Password"
3. click "Login"
4. check that page contains "Username and password do not match"

**Expected:** Error: Username and password do not match any user in this service.

---

### NEG-06: Checkout with empty First Name
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Add to cart" below "Sauce Labs Backpack"
5. scroll up
6. click "shopping cart icon" using ai
7. click "Checkout"
8. enter "Reddy" into "Last Name"
9. enter "500001" into "Zip/Postal Code"
10. click "Continue"
11. check that page contains "First Name is required"

**Expected:** Validation error: Error: First Name is required.

---

### NEG-07: Checkout with empty Last Name
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. click "Add to cart" below "Sauce Labs Backpack"
5. scroll up
6. click "shopping cart icon" using ai
7. click "Checkout"
8. enter "Vamshi" into "First Name"
9. enter "500001" into "Zip/Postal Code"
10. click "Continue"
11. check that page contains "Last Name is required"

**Expected:** Validation error: Error: Last Name is required.

---

### NEG-08: Checkout with empty Zip Code
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
10. click "Continue"
11. check that page contains "Postal Code is required"

**Expected:** Validation error: Error: Postal Code is required.

---

### NEG-09: Checkout without any items in cart
**Steps:**
1. enter "standard_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. scroll up
5. click "shopping cart icon" using ai
6. check that page contains "Your Cart"
7. click "Checkout"
8. enter "Vamshi" into "First Name"
9. enter "Reddy" into "Last Name"
10. enter "500001" into "Zip/Postal Code"
11. click "Continue"
12. check that page contains "Item total: $0.00"

**Expected:** Order overview shows $0.00 total — documents Swag Labs bug allowing empty cart checkout.

---

### NEG-10: Problem user — images load broken
**Steps:**
1. enter "problem_user" into "Username"
2. enter "secret_sauce" into "Password"
3. click "Login"
4. check that page contains "Products"
5. check that "Sauce Labs Backpack" is visible

**Expected:** Products page loads but images display incorrectly — documents a known regression indicator.
