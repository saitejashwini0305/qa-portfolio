# Requirement Traceability Matrix (RTM)

**Application:** OrangeHRM Demo  
**Module:** Login / Authentication  
**Prepared by:** Tejashwini P  
**Date:** June 2026

---

## What is an RTM?

A Requirement Traceability Matrix maps every business requirement to one or more test cases. It ensures **nothing is missed** — every requirement has been tested, and every test case has a reason to exist.

---

## RTM — Login Module

| Req ID | Requirement Description | Test Case ID | Test Case Title | Status |
|--------|------------------------|--------------|-----------------|--------|
| REQ-01 | Users must be able to log in with valid credentials | TC-LG-01 | Valid login with correct credentials | ✅ Pass |
| REQ-02 | Users must NOT be able to log in with an incorrect password | TC-LG-02 | Login with incorrect password | ✅ Pass |
| REQ-02 | Users must NOT be able to log in with an incorrect username | TC-LG-03 | Login with incorrect username | ✅ Pass |
| REQ-03 | Username field is mandatory | TC-LG-04 | Login with empty username field | ✅ Pass |
| REQ-03 | Password field is mandatory | TC-LG-05 | Login with empty password field | ✅ Pass |
| REQ-03 | Both fields mandatory — combined check | TC-LG-08 | Login with both fields empty | ✅ Pass |
| REQ-04 | Password must be masked / not shown as plain text | TC-LG-06 | Password field masks entered characters | ✅ Pass |
| REQ-05 | A "Forgot Password" link must be present and functional | TC-LG-07 | Forgot password link navigates correctly | ✅ Pass |

---

## Coverage Summary

| Requirement ID | Description | Total TCs | Passed | Failed | Coverage |
|----------------|-------------|-----------|--------|--------|----------|
| REQ-01 | Valid login | 1 | 1 | 0 | 100% |
| REQ-02 | Invalid credentials rejected | 2 | 2 | 0 | 100% |
| REQ-03 | Mandatory field validation | 3 | 3 | 0 | 100% |
| REQ-04 | Password masking | 1 | 1 | 0 | 100% |
| REQ-05 | Forgot password link | 1 | 1 | 0 | 100% |
| **Total** | | **8** | **8** | **0** | **100%** |

---

## Notes

- All 5 requirements are fully covered by the 8 test cases.
- No untested requirements (gaps) were found in this module.
- RTM will be updated if new requirements are added or test cases change.
