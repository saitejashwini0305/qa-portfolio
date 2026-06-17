# Test Cases — Login Module

**Application:** OrangeHRM Demo  
**URL:** https://opensource-demo.orangehrmlive.com/web/index.php/auth/login  
**Module:** Login / Authentication  
**Prepared by:** Tejashwini P  
**Date:** June 2026  
**Total Test Cases:** 8

---

## Requirements Covered

- Users must be able to log in with valid credentials
- Users must NOT be able to log in with invalid credentials
- Username and password fields are mandatory
- Password must be masked (not visible as plain text)
- A "Forgot Password" link must be present and functional

---

## Test Cases

### TC-LG-01 — Valid login with correct credentials

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-LG-01 |
| **Title** | Valid login with correct credentials |
| **Module** | Login |
| **Priority** | High |
| **Type** | Positive |
| **Preconditions** | User is on the login page |

**Steps to Execute:**
1. Open https://opensource-demo.orangehrmlive.com/web/index.php/auth/login
2. Enter username: `Admin`
3. Enter password: `admin123`
4. Click the "Login" button

**Expected Result:** User is redirected to the OrangeHRM dashboard successfully.  
**Actual Result:** Pass ✅  
**Status:** Pass

---

### TC-LG-02 — Login with incorrect password

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-LG-02 |
| **Title** | Login with incorrect password |
| **Module** | Login |
| **Priority** | High |
| **Type** | Negative |
| **Preconditions** | User is on the login page |

**Steps to Execute:**
1. Open the login page
2. Enter username: `Admin`
3. Enter password: `wrongpassword123`
4. Click the "Login" button

**Expected Result:** An error message "Invalid credentials" is displayed. User stays on the login page.  
**Actual Result:** Pass ✅  
**Status:** Pass

---

### TC-LG-03 — Login with incorrect username

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-LG-03 |
| **Title** | Login with incorrect username |
| **Module** | Login |
| **Priority** | High |
| **Type** | Negative |
| **Preconditions** | User is on the login page |

**Steps to Execute:**
1. Open the login page
2. Enter username: `wronguser`
3. Enter password: `admin123`
4. Click the "Login" button

**Expected Result:** An error message "Invalid credentials" is displayed. User stays on the login page.  
**Actual Result:** Pass ✅  
**Status:** Pass

---

### TC-LG-04 — Login with empty username field

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-LG-04 |
| **Title** | Login with empty username field |
| **Module** | Login |
| **Priority** | High |
| **Type** | Negative |
| **Preconditions** | User is on the login page |

**Steps to Execute:**
1. Open the login page
2. Leave the username field blank
3. Enter password: `admin123`
4. Click the "Login" button

**Expected Result:** A validation error "Required" appears below the username field.  
**Actual Result:** Pass ✅  
**Status:** Pass

---

### TC-LG-05 — Login with empty password field

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-LG-05 |
| **Title** | Login with empty password field |
| **Module** | Login |
| **Priority** | High |
| **Type** | Negative |
| **Preconditions** | User is on the login page |

**Steps to Execute:**
1. Open the login page
2. Enter username: `Admin`
3. Leave the password field blank
4. Click the "Login" button

**Expected Result:** A validation error "Required" appears below the password field.  
**Actual Result:** Pass ✅  
**Status:** Pass

---

### TC-LG-06 — Password field masks entered characters

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-LG-06 |
| **Title** | Password field masks entered characters |
| **Module** | Login |
| **Priority** | Medium |
| **Type** | Positive |
| **Preconditions** | User is on the login page |

**Steps to Execute:**
1. Open the login page
2. Click on the password field
3. Type any text (e.g. `testpassword`)
4. Observe the characters displayed in the field

**Expected Result:** Characters are masked and displayed as dots or asterisks.  
**Actual Result:** Pass ✅  
**Status:** Pass

---

### TC-LG-07 — Forgot password link navigates correctly

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-LG-07 |
| **Title** | Forgot password link navigates correctly |
| **Module** | Login |
| **Priority** | Medium |
| **Type** | Positive |
| **Preconditions** | User is on the login page |

**Steps to Execute:**
1. Open the login page
2. Locate the "Forgot your password?" link
3. Click the link

**Expected Result:** User is navigated to the password reset page.  
**Actual Result:** Pass ✅  
**Status:** Pass

---

### TC-LG-08 — Login with both fields empty

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-LG-08 |
| **Title** | Login with both fields empty |
| **Module** | Login |
| **Priority** | Low |
| **Type** | Negative |
| **Preconditions** | User is on the login page |

**Steps to Execute:**
1. Open the login page
2. Leave both username and password fields blank
3. Click the "Login" button

**Expected Result:** Validation errors "Required" appear below both the username and password fields.  
**Actual Result:** Pass ✅  
**Status:** Pass

---

## Test Summary

| Metric | Value |
|--------|-------|
| Total test cases | 8 |
| Passed | 8 |
| Failed | 0 |
| Blocked | 0 |
| Pass rate | 100% |
