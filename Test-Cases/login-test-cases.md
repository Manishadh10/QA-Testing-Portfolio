
# SauceDemo Login Test Cases

## Project Information
- **Application:** https://www.saucedemo.com/
- **Testing Type:** Manual Testing
- **Module:** Login and Logout

## Test Case Summary

| Test Case ID | Test Scenario | Expected Result | Status |
|---|---|---|---|
| TC_LOGIN_01 | Valid credentials | Products page displayed | PASS |
| TC_LOGIN_02 | Invalid username | Error message displayed | PASS |
| TC_LOGIN_03 | Invalid password | Error message displayed | PASS |
| TC_LOGIN_04 | Both fields empty | Required-field message displayed | PASS |
| TC_LOGIN_05 | Empty username | Username-required message displayed | PASS |
| TC_LOGIN_06 | Empty password | Validation message displayed | PASS |
| TC_LOGIN_07 | Both credentials invalid | Error message displayed | PASS |
| TC_LOGIN_08 | Leading space in username | Verify against requirements | INCONCLUSIVE |
| TC_LOGIN_09 | Extra password characters | Login rejected | PASS |
| TC_LOGIN_10 | Uppercase username | Login rejected | PASS |
| TC_LOGIN_11 | Uppercase password | Login rejected | PASS |
| TC_LOGIN_12 | Locked-out user | Locked-out message displayed | PASS |
| TC_LOGIN_13 | Password masking | Password hidden | PASS |
| TC_LOGIN_14 | Enter key submission | Login succeeds | PASS |
| TC_LOGIN_15 | Logout and login again | Both actions succeed | PASS |

## Execution Summary
- Passed: 14
- Failed: 0
- Inconclusive: 1
- Total test cases: 15

## Note
TC_LOGIN_08 remains inconclusive until the expected behavior
for leading spaces in usernames is confirmed.
