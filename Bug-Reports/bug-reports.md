# SAUCEDEMO LOGIN AND LOGOUT MODULE
## Comprehensive Bug Report

### 1. Project Information

| Field | Details |
|---|---|
| Project Name | SauceDemo Web Application Testing |
| Application URL | https://www.saucedemo.com/ |
| Testing Type | Manual Testing |
| Testing Level | System Testing |
| Module | Login and Logout |
| Report Type | Defect and Test Observation Report |
| Report Date | October 27, 2026 |
| Tested By | QA Tester |
| Test Environment | Web browser; browser version and OS not recorded |
| Total Test Cases | 15 |
| Passed | 14 |
| Failed | 0 |
| Inconclusive | 1 |
| Confirmed Defects | 0 |

### 2. Bug Report Terminology

| Term | Definition |
|---|---|
| Bug ID | Unique identifier assigned to a reported defect or observation. |
| Title/Summary | Short description of the issue. |
| Module | Application component being tested. |
| Severity | Degree of impact the defect has on application functionality. |
| Priority | Urgency with which the issue should be fixed. |
| Preconditions | Conditions that must be satisfied before testing. |
| Test Steps | Actions performed to reproduce the behavior. |
| Test Data | Input values used during testing. |
| Expected Result | Behavior required by the specification. |
| Actual Result | Behavior observed during test execution. |
| Status | Current state of the test or defect. |
| Reproducibility | How consistently the issue occurs. |
| Environment | Browser, operating system, device, and other relevant test conditions. |
| Evidence | Screenshots, videos, logs, or other supporting information. |
| Retest | Re-execution of a test after a correction or clarification. |
| Regression Testing | Testing existing functionality after a change to ensure it still works. |

### 3. Severity Classification

| Severity | Meaning | Example |
|---|---|---|
| Critical | System-wide failure, major security compromise, or complete loss of essential functionality. | Authentication bypass exposing protected data. |
| High | Major functionality is broken with no reasonable workaround. | All legitimate users are unable to log in. |
| Medium | Significant functionality is affected, but a workaround may exist. | Valid login fails under a particular supported condition. |
| Low | Minor functional issue with limited impact. | Incorrect validation message or a minor input-handling issue. |
| Trivial | Cosmetic issue with negligible functional impact. | Slight alignment issue on the login page. |

### 4. Priority Classification

| Priority | Meaning |
|---|---|
| P1 – Critical | Immediate attention required. |
| P2 – High | Fix urgently in the next appropriate release or development cycle. |
| P3 – Medium | Fix under normal development scheduling. |
| P4 – Low | Fix when resources permit. |

**Important:** Severity measures the impact of a defect, while priority measures how urgently it should be addressed. Severity and priority are not assigned to passed tests. An inconclusive test should normally remain unclassified until its behavior is investigated.

---

# 5. Detailed Test Case and Bug Assessment Records

## TC_LOGIN_01 – Valid Credentials

**Bug ID:** No defect identified

- **Module:** Login
- **Severity:** N/A
- **Priority:** N/A
- **Status:** PASS
- **Reproducibility:** Passed in the recorded execution

**Preconditions**
1. The application is accessible.
2. A valid test account is available.

**Test Steps**
1. Open the SauceDemo login page.
2. Enter valid login credentials.
3. Click Login.

**Test Data:** Valid username and password.

**Expected Result:** The user is authenticated and redirected to the Products page.

**Actual Result:** The Products page was displayed according to the test result.

**Impact:** No defect identified.

**Recommended Action:** No corrective action required. Retain the test as a regression test.

---

## TC_LOGIN_02 – Invalid Username

**Bug ID:** No defect identified

- **Module:** Login
- **Severity:** N/A
- **Priority:** N/A
- **Status:** PASS

**Preconditions:** The login page is accessible.

**Test Steps**
1. Open the login page.
2. Enter an invalid username.
3. Enter a password.
4. Click Login.

**Test Data:** Invalid username and a password.

**Expected Result:** Authentication is rejected and an appropriate error message is displayed.

**Actual Result:** The test was recorded as passed; the exact error text was not documented.

**Impact:** No defect identified.

**Recommended Action:** No fix required. Record the exact error message in future execution evidence.

---

## TC_LOGIN_03 – Invalid Password

**Bug ID:** No defect identified

- **Module:** Login
- **Severity:** N/A
- **Priority:** N/A
- **Status:** PASS

**Preconditions:** A valid username is available.

**Test Steps**
1. Open the login page.
2. Enter a valid username.
3. Enter an incorrect password.
4. Click Login.

**Test Data:** Valid username and invalid password.

**Expected Result:** Login is rejected and an appropriate error message is displayed.

**Actual Result:** The test was recorded as passed.

**Impact:** No defect identified.

**Recommended Action:** No corrective action required.

---

## TC_LOGIN_04 – Both Fields Empty

**Bug ID:** No defect identified

- **Module:** Login
- **Severity:** N/A
- **Priority:** N/A
- **Status:** PASS

**Preconditions:** The login page is accessible.

**Test Steps**
1. Open the login page.
2. Leave the username field empty.
3. Leave the password field empty.
4. Click Login.

**Test Data:** Username: empty; Password: empty.

**Expected Result:** The application prevents login and displays the required-field validation message.

**Actual Result:** The test was recorded as passed.

**Impact:** No defect identified.

**Recommended Action:** No corrective action required.

---

## TC_LOGIN_05 – Empty Username

**Bug ID:** No defect identified

- **Module:** Login
- **Severity:** N/A
- **Priority:** N/A
- **Status:** PASS

**Preconditions:** The login page is accessible.

**Test Steps**
1. Open the login page.
2. Leave the username field empty.
3. Enter a password.
4. Click Login.

**Test Data:** Empty username and a password.

**Expected Result:** Login is rejected and a username-required validation message is displayed.

**Actual Result:** The test was recorded as passed.

**Impact:** No defect identified.

**Recommended Action:** No corrective action required.

---

## TC_LOGIN_06 – Empty Password

**Bug ID:** No defect identified

- **Module:** Login
- **Severity:** N/A
- **Priority:** N/A
- **Status:** PASS

**Preconditions:** The login page is accessible.

**Test Steps**
1. Open the login page.
2. Enter a username.
3. Leave the password field empty.
4. Click Login.

**Test Data:** Username entered; password empty.

**Expected Result:** Login is rejected and the appropriate validation message is displayed.

**Actual Result:** The test was recorded as passed.

**Impact:** No defect identified.

**Recommended Action:** No corrective action required.

---

## TC_LOGIN_07 – Both Credentials Invalid

**Bug ID:** No defect identified

- **Module:** Login
- **Severity:** N/A
- **Priority:** N/A
- **Status:** PASS

**Preconditions:** The login page is accessible.

**Test Steps**
1. Open the login page.
2. Enter an invalid username.
3. Enter an invalid password.
4. Click Login.

**Test Data:** Invalid username and invalid password.

**Expected Result:** Authentication is rejected and an appropriate error message is displayed.

**Actual Result:** The test was recorded as passed.

**Impact:** No defect identified.

**Recommended Action:** No corrective action required.

---

## TC_LOGIN_08 – Leading Space in Username

**Observation ID:** OBS_LOGIN_001

- **Module:** Login
- **Severity:** TBD – Not assessed
- **Priority:** TBD – Not assessed
- **Status:** INCONCLUSIVE
- **Defect Confirmed:** No
- **Reproducibility:** Not established

**Preconditions**
1. The login page is accessible.
2. A valid username and corresponding password are available.

**Test Steps**
1. Open the login page.
2. Enter a valid username preceded by a space.
3. Enter the corresponding password.
4. Click Login.
5. Observe the application's response.

**Test Data:** Valid username with a leading space and its corresponding password.

**Expected Result:** The application should handle leading spaces according to the approved input-validation requirements.

**Actual Result:** The actual behavior has not been established from the supplied test record.

**Impact:** Username input handling remains unverified.

**Recommended Action**
1. Confirm whether leading spaces should be trimmed or rejected.
2. Repeat the test using the approved expected behavior.
3. Capture the actual response and supporting screenshot.
4. Mark the test PASS or FAIL based on the result.

**Defect classification:** This is an unresolved test observation, not a confirmed bug. Severity and priority should be assigned only if a defect is verified.

---

## TC_LOGIN_09 – Extra Password Characters

**Bug ID:** No defect identified

- **Module:** Login
- **Severity:** N/A
- **Priority:** N/A
- **Status:** PASS

**Preconditions:** A valid username and password are available.

**Test Steps**
1. Open the login page.
2. Enter a valid username.
3. Enter the correct password with additional characters.
4. Click Login.

**Test Data:** Valid username and modified password.

**Expected Result:** Login is rejected because the password does not match the valid credentials.

**Actual Result:** The test was recorded as passed.

**Impact:** No defect identified.

**Recommended Action:** No corrective action required.

---

## TC_LOGIN_10 – Uppercase Username

**Bug ID:** No defect identified

- **Module:** Login
- **Severity:** N/A
- **Priority:** N/A
- **Status:** PASS

**Preconditions:** A valid username is available.

**Test Steps**
1. Open the login page.
2. Convert the username to uppercase.
3. Enter the corresponding password.
4. Click Login.

**Test Data:** Uppercase username and corresponding password.

**Expected Result:** For the stated test scenario, login is rejected when the uppercase username does not match the accepted username.

**Actual Result:** The test was recorded as passed.

**Impact:** No defect identified.

**Recommended Action:** No corrective action required. Confirm that the expected case sensitivity matches the application's requirements.

---

## TC_LOGIN_11 – Uppercase Password

**Bug ID:** No defect identified

- **Module:** Login
- **Severity:** N/A
- **Priority:** N/A
- **Status:** PASS

**Preconditions:** A valid username and password are available.

**Test Steps**
1. Open the login page.
2. Enter a valid username.
3. Convert the password to uppercase.
4. Click Login.

**Test Data:** Valid username and uppercase version of the password.

**Expected Result:** Login is rejected when the modified password does not match the valid password.

**Actual Result:** The test was recorded as passed.

**Impact:** No defect identified.

**Recommended Action:** No corrective action required.

---

## TC_LOGIN_12 – Locked-Out User

**Bug ID:** No defect identified

- **Module:** Login
- **Severity:** N/A
- **Priority:** N/A
- **Status:** PASS

**Preconditions:** A designated locked-out test account is available.

**Test Steps**
1. Open the login page.
2. Enter the locked-out user's credentials.
3. Click Login.
4. Observe the displayed message.

**Test Data:** Credentials for the designated locked-out user.

**Expected Result:** Login is prevented and the appropriate locked-out message is displayed.

**Actual Result:** The test was recorded as passed.

**Impact:** No defect identified.

**Recommended Action:** No corrective action required.

---

## TC_LOGIN_13 – Password Masking

**Bug ID:** No defect identified

- **Module:** Login
- **Severity:** N/A
- **Priority:** N/A
- **Status:** PASS

**Preconditions:** The login page is accessible.

**Test Steps**
1. Open the login page.
2. Enter a password.
3. Observe how the password is displayed.

**Test Data:** Any permitted test password.

**Expected Result:** Password characters are visually masked in the password field.

**Actual Result:** The test was recorded as passed.

**Impact:** No defect identified.

**Recommended Action:** No corrective action required. Note that visual masking alone does not establish the security of password storage or transmission.

---

## TC_LOGIN_14 – Enter Key Submission

**Bug ID:** No defect identified

- **Module:** Login
- **Severity:** N/A
- **Priority:** N/A
- **Status:** PASS

**Preconditions:** Valid credentials are available.

**Test Steps**
1. Open the login page.
2. Enter a valid username.
3. Enter a valid password.
4. Press Enter instead of clicking Login.
5. Observe the result.

**Test Data:** Valid username and password.

**Expected Result:** The form is submitted and the user is redirected to the Products page.

**Actual Result:** The test was recorded as passed.

**Impact:** No defect identified.

**Recommended Action:** No corrective action required. Retain this test for keyboard-accessibility and regression testing.

---

## TC_LOGIN_15 – Logout and Login Again

**Bug ID:** No defect identified

- **Module:** Login and Logout
- **Severity:** N/A
- **Priority:** N/A
- **Status:** PASS

**Preconditions**
1. The user has valid credentials.
2. The user can access the application after login.

**Test Steps**
1. Log in using valid credentials.
2. Navigate to the application menu.
3. Select Logout.
4. Verify that the login page is displayed.
5. Log in again using valid credentials.

**Test Data:** Valid username and password.

**Expected Result:** Logout returns the user to the login page, and a subsequent valid login succeeds.

**Actual Result:** Both logout and subsequent login were recorded as successful.

**Impact:** No defect identified.

**Recommended Action:** No corrective action required. Consider additional tests for browser Back navigation and session behavior after logout.

---

# 6. Consolidated Defect Assessment Table

| Test Case ID | Bug/Observation ID | Scenario | Severity | Priority | Status |
|---|---|---|---|---|---|
| TC_LOGIN_01 | None | Valid credentials | N/A | N/A | PASS |
| TC_LOGIN_02 | None | Invalid username | N/A | N/A | PASS |
| TC_LOGIN_03 | None | Invalid password | N/A | N/A | PASS |
| TC_LOGIN_04 | None | Both fields empty | N/A | N/A | PASS |
| TC_LOGIN_05 | None | Empty username | N/A | N/A | PASS |
| TC_LOGIN_06 | None | Empty password | N/A | N/A | PASS |
| TC_LOGIN_07 | None | Both credentials invalid | N/A | N/A | PASS |
| TC_LOGIN_08 | OBS_LOGIN_001 | Leading space in username | TBD | TBD | INCONCLUSIVE |
| TC_LOGIN_09 | None | Extra password characters | N/A | N/A | PASS |
| TC_LOGIN_10 | None | Uppercase username | N/A | N/A | PASS |
| TC_LOGIN_11 | None | Uppercase password | N/A | N/A | PASS |
| TC_LOGIN_12 | None | Locked-out user | N/A | N/A | PASS |
| TC_LOGIN_13 | None | Password masking | N/A | N/A | PASS |
| TC_LOGIN_14 | None | Enter key submission | N/A | N/A | PASS |
| TC_LOGIN_15 | None | Logout and login again | N/A | N/A | PASS |

# 7. Execution Summary

| Execution Metric | Count |
|---|---:|
| Total test cases | 15 |
| Passed test cases | 14 |
| Failed test cases | 0 |
| Inconclusive test cases | 1 |
| Confirmed defects | 0 |
| Unresolved observations | 1 |

**Pass rate:** 93.33% (14 out of 15 test cases).

**Fail rate:** 0% (0 out of 15 test cases).

**Inconclusive rate:** 6.67% (1 out of 15 test cases).

# 8. Bug Reporting and Retesting Workflow

1. **Identification:** Identify unexpected behavior during test execution.
2. **Documentation:** Record the bug ID, summary, environment, steps, expected result, actual result, severity, priority, and evidence.
3. **Submission:** Submit the verified defect to the development or defect-tracking team.
4. **Triage:** The QA lead and development team confirm severity, priority, ownership, and whether the issue is reproducible.
5. **Fix:** The developer investigates and corrects the defect.
6. **Retesting:** QA repeats the original test case against the corrected application.
7. **Regression testing:** QA tests related features to check for unintended side effects.
8. **Closure:** Close the defect if the correction is verified; otherwise, reopen it.

Typical defect lifecycle statuses include **New, Assigned, Open, In Progress, Fixed, Ready for Retest, Reopened, Deferred, Rejected, and Closed**. Exact status names depend on the team's defect-tracking process.

# 9. Final Conclusion

Manual testing of the SauceDemo Login and Logout module covered 15 test cases involving valid and invalid credentials, empty fields, password handling, locked-out users, keyboard submission, and logout functionality.

Fourteen test cases passed, no test cases failed, and one test case remains inconclusive. The supplied execution results do not establish any confirmed application defects.

The next action is to clarify and retest TC_LOGIN_08. After that test is resolved, the QA team can finalize the execution report and determine whether any actual defects require severity and priority classification.

**Report prepared for:** SauceDemo Login and Logout Manual Testing  
**Report status:** Pending clarification of TC_LOGIN_08

*Evidence limitation: Actual screenshots, browser details, exact validation messages, and independent execution logs were not supplied. The actual-result descriptions above reflect the provided test summary and should not be treated as independently verified observations.*
