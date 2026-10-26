
# SauceDemo Bug Report

## Project Information

- **Project:** SauceDemo Manual QA Testing
- **Application:** https://www.saucedemo.com/
- **Testing Type:** Manual Testing
- **Module:** Login and Logout

---

## Bug Report Summary

| Field | Details |
|---|---|
| Total Test Cases Executed | 15 |
| Confirmed Bugs Identified | 0 |
| Open Bugs | 0 |
| Note | One test case remains inconclusive |

No confirmed defects were identified during the recorded test execution. TC_LOGIN_08 remains inconclusive because the expected handling of leading spaces in usernames has not been confirmed.

---

## Bug Report Template

Use this template if a defect is identified during future testing.

### Bug ID
BUG_LOGIN_001

### Bug Title
[Short and clear description of the defect]

### Module
Login / Logout

### Environment
- Operating System: [Enter actual OS]
- Browser: [Enter browser and version]
- Test Date: [Enter test date]

### Preconditions
[Describe the conditions required before testing.]

### Steps to Reproduce
1. Open https://www.saucedemo.com/
2. [Enter the action that triggers the defect.]
3. [Continue with the reproduction steps.]
4. Observe the behavior.

### Expected Result
[Describe the behavior required by the specification.]

### Actual Result
[Describe what actually happened.]

### Severity
[Critical / High / Medium / Low]

### Priority
[High / Medium / Low]

### Status
[New / Open / In Progress / Fixed / Closed]

### Evidence
[Attach a screenshot or recording if available.]

---

## Inconclusive Test Follow-up

### Reference
TC_LOGIN_08 — Username with leading spaces

- **Test Data:** Username ` standard_user`, password `secret_sauce`
- **Observed Result:** Login was rejected with an invalid credentials message.
- **Expected Behavior:** Not yet established.
- **Status:** Inconclusive; not currently classified as a defect.
- **Next Action:** Confirm whether the requirements specify trimming leading spaces before deciding whether to raise a bug.

---

## Conclusion

This file records the current bug-reporting status and provides a reusable template for future verified defects. A bug should be reported only when the actual behavior conflicts with an established requirement or expected behavior.
