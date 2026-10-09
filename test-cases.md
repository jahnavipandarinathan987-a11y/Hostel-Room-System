
# HostelHub — Test Case Report

## Project Details
- **Project:** Hostel Room Management System
- **Application:** HostelHub
- **Test Type:** Manual Functional Testing
- **Environment:** Windows laptop, web browser
- **Test Approach:** Positive, negative, boundary, and validation testing

## Test Cases and Execution Results

| Test ID | Test Scenario | Expected Result | Actual Result | Status |
|---|---|---|---|---|
| TC-01 | Sign in with a student ID and name | Student session is displayed | Sign-in succeeded and header displayed the student name | PASS |
| TC-02 | Allocate a bed in a room with availability | Occupancy increases and available beds decrease | Room occupancy increased and available beds decreased | PASS |
| TC-03 | Submit a valid room application | Application is saved with Pending status | Application submitted and appeared in the status table | PASS |
| TC-04 | Submit an application with an empty reason | Submission is blocked by required-field validation | Browser blocked submission | PASS |
| TC-05 | Attempt to allocate a bed when the room is full | No further allocation is permitted | Full room showed no allocation button | PASS |
| TC-06 | Submit a second application while one is pending for the same student | Duplicate pending application is rejected | Duplicate application was rejected | PASS |

## Test Summary

- Total test cases executed: 6
- Passed: 6
- Failed: 0
- Test type: Manual functional testing
- Overall result: All six recorded checks passed.

## Limitations

- Testing was performed on a local browser-based prototype.
- The application uses browser local storage rather than a shared backend database.
- Student login is a demonstration flow and does not implement secure authentication.
- These results do not establish automated test coverage, unit-test coverage, or performance under concurrent users.
- Test results reflect the scenarios manually executed during this test session.

## Future Testing

1. Test malformed and excessively long input values.
2. Verify persistence after refreshing and reopening the browser.
3. Add automated unit tests for room allocation and application validation.
4. Add automated UI testing for the student login and application workflow.
5. Measure code coverage and cyclomatic complexity.
6. Test integration against a backend database when implemented.
