# BUG-009 — Login succeeds with empty Email and Password fields

**Severity:** Major

**Environment:**
- Web Application
- Google Chrome
- Windows 11

**Preconditions:**
User is on the login page.

**Steps to Reproduce:**
1. Leave the Email field empty.
2. Leave the Password field empty.
3. Click **Log In**.

**Test Data:**
- Email: empty
- Password: empty

**Expected Result:**
Login should be rejected and the user should not be logged in.

**Actual Result:**
Login is successful and the user is redirected to the Account Page.
