# 01 — Manual Testing

**Application Under Test:** OrangeHRM Demo (https://opensource-demo.orangehrmlive.com)  
**Module Tested:** Login / Authentication  
**Tester:** Tejashwini P  
**Completed:** June 2026

---

## Overview

This section demonstrates manual testing skills including test case design, test execution, requirements traceability, and defect reporting — all performed against the OrangeHRM open-source HR application.

---

## Artifacts

| File | Description |
|------|-------------|
| [test-cases-login.md](./test-cases-login.md) | 8 test cases covering the login module with steps, expected results, and execution status |
| [RTM.md](./RTM.md) | Requirement Traceability Matrix mapping all 5 requirements to their test cases |
| [bug-report-template.md](./bug-report-template.md) | Professional bug report template with a filled example and severity guide |
| [screenshots/](./screenshots/) | Evidence screenshots captured during test execution |

---

## Test Execution Summary

| Module | Total TCs | Passed | Failed | Pass Rate |
|--------|-----------|--------|--------|-----------|
| Login | 8 | 8 | 0 | 100% |

---

## Testing Approach

**Test types applied:**
- Functional testing — verifying features work as specified
- Negative testing — verifying the app handles invalid inputs gracefully
- Boundary testing — empty fields, invalid credentials
- UI validation — field masking, link navigation

**Test design techniques used:**
- Equivalence partitioning (valid vs. invalid credential classes)
- Boundary value analysis (empty fields)
- Requirement-based testing (each requirement maps to at least one test case)

---

## Tools Used

| Tool | Purpose |
|------|---------|
| OrangeHRM Demo | Application under test |
| Markdown / GitHub | Test artifact documentation |
| Chrome DevTools | Browser environment for execution |
| JIRA (template) | Bug report format reference |
