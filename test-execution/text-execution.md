# Test Execution — Web Registration & Login

> **Note:** Test execution results are simulated for learning and portfolio purposes. No real commercial application was tested.

## Execution Results

| Test Case | Actual Result | Status | Bug ID |
|---|---|---|---|
| TC-001 | Registration completed successfully and user was redirected to the Account Page. | PASS | N/A |
| TC-002 | Registration was rejected and the user was informed that the password must contain at least 8 characters. | PASS | N/A |
| TC-003 | Registration was completed successfully despite mismatched passwords. | FAIL | BUG-002 |
| TC-004 | Registration was completed successfully with an empty Email field. | FAIL | BUG-003 |
| TC-005 | Registration completed successfully with an exactly 8-character password. | PASS | N/A |
| TC-006 | Registration was completed successfully with empty Password and Confirm Password fields. | FAIL | BUG-007 |
| TC-007 | Registration was completed successfully with an empty Confirm Password field. | FAIL | BUG-006 |
| TC-008 | The user was informed that the email format was invalid. No defect was observed against the defined requirements. | PASS | N/A |
| TC-009 | Registration completed successfully with a 9-character password. | PASS | N/A |
| TC-010 | Registration was completed successfully despite mismatched Password and Confirm Password fields. | FAIL | BUG-002 |
| TC-011 | Login was successful with valid credentials and the user was redirected to the Account Page. | PASS | N/A |
| TC-012 | Login was successful with invalid credentials. | FAIL | BUG-004 |
| TC-013 | Login was successful with an empty Email field. | FAIL | BUG-008 |
| TC-014 | Login was successful with an empty Password field. | FAIL | BUG-005 |
| TC-015 | Login was successful with empty Email and Password fields. | FAIL | BUG-009 |

---

## Test Summary

| Metric | Result |
|---|---:|
| Total Test Cases | 15 |
| Passed | 6 |
| Failed | 9 |
| Blocked | 0 |

### Pass Rate

**40%**

### Fail Rate

**60%**

---

## Execution Analysis

The simulated test execution identified functional issues in both registration and login functionality.

### Registration

The following issues were identified:

- Password length validation does not prevent a 7-character password.
- Registration accepts mismatched passwords.
- Registration accepts an empty Email field.
- Registration accepts empty Password and Confirm Password fields.
- Registration accepts an empty Confirm Password field.

### Login

The following issues were identified:

- Invalid credentials allow login.
- Empty Email allows login.
- Empty Password allows login.
- Empty Email and Password allow login.

---

## Notes

TC-008 was treated as PASS because the project requirements define Email as a required field but do not explicitly define email format validation.

The test execution results are simulated and are intended to demonstrate the QA testing process, test result analysis, and bug-reporting workflow.
