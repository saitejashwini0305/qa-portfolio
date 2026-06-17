# Bug Report Template & Example

**Application:** OrangeHRM Demo  
**Module:** Login / Authentication  
**Prepared by:** Tejashwini P

---

## Bug Report Template

Use this template for every bug you find. Copy it and fill in each field.

```
## BUG-[ID] — [Short title describing what is broken]

| Field | Details |
|-------|---------|
| **Bug ID** | BUG-XXX |
| **Title** | [What broke] + [where] + [under what condition] |
| **Module** | [Which part of the app] |
| **Severity** | Critical / Major / Minor / Trivial |
| **Priority** | High / Medium / Low |
| **Status** | New / Open / In Progress / Fixed / Closed |
| **Reported by** | [Your name] |
| **Date** | [Date found] |
| **Environment** | Browser: ___ | OS: ___ | App version: ___ |
| **Test Case Ref** | TC-XX-XX |

### Steps to Reproduce
1. Step one (be exact — include URLs, field values, button names)
2. Step two
3. Step three

### Expected Result
[What should happen according to the requirement]

### Actual Result
[What actually happened — factual, no opinions]

### Attachments
- [ ] Screenshot
- [ ] Screen recording
- [ ] Console logs (if applicable)
```

---

## Severity Level Guide

| Severity | Definition | Example |
|----------|------------|---------|
| **Critical** | App crashes, data loss, security issue, or core feature completely broken | Login page shows blank white screen |
| **Major** | Key feature broken but app still usable | Error message not shown on wrong password |
| **Minor** | Feature works but behaves unexpectedly | Button label has a typo |
| **Trivial** | Cosmetic issue with no functional impact | Logo is slightly misaligned on mobile |

---

## Example Bug Report (Filled In)

> This is a sample bug report written for practice. In a real project this would
> be logged in JIRA or a similar tool. OrangeHRM's login currently passes all
> test cases — this is a hypothetical example showing the correct format.

---

## BUG-001 — Error message not displayed when user enters incorrect password on login page

| Field | Details |
|-------|---------|
| **Bug ID** | BUG-001 |
| **Title** | Error message not displayed when user enters incorrect password on login page |
| **Module** | Login / Authentication |
| **Severity** | Major |
| **Priority** | High |
| **Status** | New |
| **Reported by** | Tejashwini P |
| **Date** | June 2026 |
| **Environment** | Browser: Chrome 125 \| OS: Windows 11 \| App: OrangeHRM Demo |
| **Test Case Ref** | TC-LG-02 |

### Steps to Reproduce
1. Open https://opensource-demo.orangehrmlive.com/web/index.php/auth/login
2. Enter username: `Admin`
3. Enter password: `wrongpassword123`
4. Click the "Login" button

### Expected Result
An error message such as "Invalid credentials" should appear below the login form.
The user should remain on the login page.

### Actual Result
No error message is displayed. The page refreshes silently and the user remains
on the login page with no feedback indicating what went wrong.

### Impact
Users have no way of knowing their credentials were incorrect. This could lead
to confusion, repeated failed attempts, and potential account lockout without
clear guidance.

### Attachments
- [ ] Screenshot — `screenshots/BUG-001-no-error-message.png`

---

## Bug ID Naming Convention

| Component | Format | Example |
|-----------|--------|---------|
| Bug ID | `BUG-[number]` | BUG-001 |
| Test case link | `TC-[module]-[number]` | TC-LG-02 |
| Screenshot | `BUG-[id]-[short-desc].png` | BUG-001-no-error-message.png |

---

## Notes for Your Portfolio

When you find real bugs in future testing:
1. Copy the template above
2. Create a new file: `bug-reports/BUG-XXX-short-title.md`
3. Add your screenshot to the `screenshots/` folder
4. Reference the bug ID in your test execution report
