# Bug Reports — Web Registration & Login

> Demo QA project created for portfolio purposes. The reported defects are simulated for learning purposes.

## BUG-001 — Registration accepts a 7-character password

**Severity:** Major

**Environment:**
- Web Application
- Google Chrome
- Windows 11

**Preconditions:**
User is on the registration page.

**Steps to Reproduce:**
1. Enter a valid email address.
2. Enter a 7-character password.
3. Enter the same password in the Confirm Password field.
4. Click **Sign Up**.

**Test Data:**
- Email: `test@example.com`
- Password: `test123`
- Confirm Password: `test123`

**Expected Result:**
Registration should be rejected and the user should be informed that the password must contain at least 8 characters.

**Actual Result:**
Registration is completed successfully and the user is redirected to the Account Page.

---

## BUG-002 — Registration accepts mismatched passwords

**Severity:** Major

**Environment:**
- Web Application
- Google Chrome
- Windows 11

**Preconditions:**
User is on the registration page.

**Steps to Reproduce:**
1. Enter a valid email address.
2. Enter a valid password.
3. Enter a different value in the Confirm Password field.
4. Click **Sign Up**.

**Test Data:**
- Email: `test@example.com`
- Password: `Test1234!`
- Confirm Password: `Test12345!`

**Expected Result:**
Registration should be rejected and the user should be informed that the passwords must match.

**Actual Result:**
Registration is completed successfully and the user is redirected to the Account Page.

---

## BUG-003 — Registration accepts an empty Email field

**Severity:** Major

**Environment:**
- Web Application
- Google Chrome
- Windows 11

**Preconditions:**
User is on the registration page.

**Steps to Reproduce:**
1. Leave the Email field empty.
2. Enter a valid password.
3. Enter the same password in the Confirm Password field.
4. Click **Sign Up**.

**Test Data:**
- Email: empty
- Password: `Test1234!`
- Confirm Password: `Test1234!`

**Expected Result:**
Registration should be rejected and the user should be informed that Email is required.

**Actual Result:**
Registration is completed successfully and the user is redirected to the Account Page.

---

## BUG-004 — Login succeeds with invalid credentials

**Severity:** Major

**Environment:**
- Web Application
- Google Chrome
- Windows 11

**Preconditions:**
User is on the login page.

**Steps to Reproduce:**
1. Enter a valid email address.
2. Enter an incorrect password.
3. Click **Log In**.

**Test Data:**
- Email: `test@example.com`
- Password: `WrongPassword123`

**Expected Result:**
Login should be rejected and the user should not be logged in.

**Actual Result:**
Login is successful and the user is redirected to the Account Page.

---

## BUG-005 — Login succeeds with an empty Password field

**Severity:** Major

**Environment:**
- Web Application
- Google Chrome
- Windows 11

**Preconditions:**
User is on the login page.

**Steps to Reproduce:**
1. Enter a valid email address.
2. Leave the Password field empty.
3. Click **Log In**.

**Test Data:**
- Email: `test@example.com`
- Password: empty

**Expected Result:**
Login should be rejected and the user should not be logged in.

**Actual Result:**
Login is successful and the user is redirected to the Account Page.

---

## BUG-006 — Registration accepts empty Confirm Password field

**Severity:** Major

**Environment:**
- Web Application
- Google Chrome
- Windows 11

**Preconditions:**
User is on the registration page.

**Steps to Reproduce:**
1. Enter a valid email address.
2. Enter a valid password.
3. Leave the Confirm Password field empty.
4. Click **Sign Up**.

**Test Data:**
- Email: `test@example.com`
- Password: `Test1234!`
- Confirm Password: empty

**Expected Result:**
Registration should be rejected and the user should be informed that Confirm Password is required.

**Actual Result:**
Registration is completed successfully and the user is redirected to the Account Page.

---

## BUG-007 — Registration succeeds with empty Password and Confirm Password fields

**Severity:** Major

**Environment:**
- Web Application
- Google Chrome
- Windows 11

**Preconditions:**
User is on the registration page.

**Steps to Reproduce:**
1. Enter a valid email address.
2. Leave the Password field empty.
3. Leave the Confirm Password field empty.
4. Click **Sign Up**.

**Test Data:**
- Email: `test@example.com`
- Password: empty
- Confirm Password: empty

**Expected Result:**
Registration should be rejected and the user should be informed that Password is required.

**Actual Result:**
Registration is completed successfully and the user is redirected to the Account Page.

---

## BUG-008 — Login succeeds with an empty Email field

**Severity:** Major

**Environment:**
- Web Application
- Google Chrome
- Windows 11

**Preconditions:**
User is on the login page.

**Steps to Reproduce:**
1. Leave the Email field empty.
2. Enter a valid password.
3. Click **Log In**.

**Test Data:**
- Email: empty
- Password: `Test1234!`

**Expected Result:**
Login should be rejected and the user should not be logged in.

**Actual Result:**
Login is successful and the user is redirected to the Account Page.
