# Registration Test Cases

## Test Environment

**Application:** nopCommerce Demo Store
**Test Type:** Manual Functional Testing
**Testing Area:** User Registration

---

## TC-REG-001 — Successful User Registration

**Objective:**
Verify that a new user can successfully register using valid information.

**Preconditions:**

* User is not logged in.
* A unique email address is available.

**Test Steps:**

1. Navigate to the registration page.
2. Enter a valid first name.
3. Enter a valid last name.
4. Enter a unique valid email address.
5. Enter a valid password.
6. Confirm the password.
7. Click Register.

**Expected Result:**
The user should be successfully registered.

**Actual Result:**
The user registration completed successfully.

**Status:** PASS

---

## TC-REG-002 — Required Field Validation

**Objective:**
Verify that registration cannot be completed when required fields are empty.

**Test Steps:**

1. Navigate to the registration page.
2. Leave all required fields blank.
3. Click Register.

**Expected Result:**
Registration should be prevented and validation messages should be displayed for the required fields.

**Actual Result:**
The application prevented registration and displayed validation errors.

**Status:** PASS

---

## TC-REG-003 — Invalid Email Format

**Objective:**
Verify that the application rejects an invalid email address.

**Test Data:**

`qa-test`

**Test Steps:**

1. Navigate to the registration page.
2. Enter valid information in the required fields.
3. Enter `qa-test` in the email field.
4. Click Register.

**Expected Result:**
The application should reject the invalid email format and display an appropriate validation message.

**Actual Result:**
The application rejected the invalid email address and displayed:

> Please enter a valid email address.

**Status:** PASS

---

## TC-REG-004 — Password Below Minimum Length

**Objective:**
Verify that passwords shorter than the minimum required length are rejected.

**Test Data:**

`123`

**Test Steps:**

1. Enter valid registration information.
2. Enter `123` as the password.
3. Enter `123` as the confirmation password.
4. Submit the form.

**Expected Result:**
The application should reject the password because it does not meet the minimum length requirement.

**Actual Result:**
The application rejected the password and displayed:

> Password must meet the following rules: must have at least 6 characters and not greater than 64 characters

**Status:** PASS

---

## TC-REG-005 — Minimum Valid Password

**Objective:**
Verify that a password containing exactly six characters is accepted.

**Test Data:**

`123456`

**Test Steps:**

1. Enter valid registration information.
2. Enter `123456` as the password.
3. Enter `123456` as the confirmation password.
4. Submit the form.

**Expected Result:**
A six-character password should be accepted because the application specifies a minimum length of six characters.

**Actual Result:**
The six-character password was accepted and registration completed successfully.

**Status:** PASS

---

## TC-REG-006 — Password Confirmation Mismatch

**Objective:**
Verify that registration is prevented when the password and confirmation password do not match.

**Test Data:**

Password: `123456`
Confirm Password: `123457`

**Test Steps:**

1. Enter valid registration information.
2. Enter `123456` as the password.
3. Enter `123457` as the confirmation password.
4. Submit the registration form.

**Expected Result:**
Registration should be prevented and an appropriate password mismatch validation message should be displayed.

**Actual Result:**
Error message: "The password and confirmation password do not match." is returned successfully

**Status:** PASS
