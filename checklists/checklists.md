# Checklists — Web Registration & Login

## Registration Checklist

- [ ] Email field is required
- [ ] Password field is required
- [ ] Confirm Password field is required
- [ ] Password must contain at least 8 characters
- [ ] Password with 7 characters is rejected
- [ ] Password with exactly 8 characters is accepted
- [ ] Password with 9 characters is accepted
- [ ] Password and Confirm Password must match
- [ ] Mismatched passwords are rejected
- [ ] Empty Email is rejected
- [ ] Invalid email format is handled according to defined requirements
- [ ] Successful registration redirects the user to the Account Page

---

## Login Checklist

- [ ] Email field is required
- [ ] Password field is required
- [ ] Valid credentials allow login
- [ ] Invalid credentials do not allow login
- [ ] Empty Email is rejected
- [ ] Empty Password is rejected
- [ ] Empty Email and Password are rejected
- [ ] Invalid password does not allow login
- [ ] User is not logged in after failed authentication

---

## Notes

This checklist is based on the defined project requirements.

The email format validation requirement is not explicitly defined, so expected behavior should be clarified before treating a specific email-format behavior as a defect.
