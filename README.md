# E-Commerce Web Application — Manual QA Testing

## 📋 Project Overview

This project demonstrates manual software testing of an e-commerce web application. The objective is to evaluate core user workflows, identify defects, validate input handling, and document testing results using industry-style QA artifacts.

## 🎯 Testing Objectives

* Validate user registration functionality
* Verify form validation and error handling
* Perform positive and negative testing
* Perform boundary-value testing
* Document test cases and execution results
* Capture testing evidence
* Identify and document software defects

## 🧪 Testing Scope

### Registration

* Valid user registration
* Required field validation
* Invalid email validation
* Password length validation
* Password confirmation validation
* Password boundary testing

### Login

* Valid login
* Invalid credentials
* Empty fields
* Logout

### Product & Search

* Product search
* Category navigation
* Product details
* Invalid/nonexistent searches

### Shopping Cart

* Add product
* Remove product
* Quantity changes
* Price validation

### Checkout

* Required field validation
* Invalid input
* Successful checkout flow

## 🛠️ Testing Approach

The project uses:

* Functional Testing
* Positive Testing
* Negative Testing
* Boundary Value Analysis
* Exploratory Testing
* Regression Testing
* Test Case Design
* Defect Documentation

## 📊 Test Results

Initial registration testing has been completed and documented in the test case repository.

| Test ID    | Test Area                     | Result  |
| ---------- | ----------------------------- | ------- |
| TC-REG-001 | Valid Registration            | PASS    |
| TC-REG-002 | Required Field Validation     | PASS    |
| TC-REG-003 | Invalid Email                 | PASS    |
| TC-REG-004 | Password Below Minimum Length | PASS    |
| TC-REG-005 | Minimum Valid Password        | PASS    |
| TC-REG-006 | Password Confirmation         | PASS    |

## 📁 Project Structure

```text
qa-ecommerce-manual-testing/
│
├── README.md
│
├── Test-Cases/
│   └── Test-Cases.md
│
├── Bug-Reports/
│
├── Test-Execution/
│
└── Evidence/
    └── screenshots/
```

## 🔍 Evidence

Screenshots and other testing evidence are stored in the `Evidence` directory and are linked to the applicable test cases.

## 📌 Notes

Testing is performed against a publicly available demonstration e-commerce application. Results documented in this repository represent the behavior observed during the testing sessions.
