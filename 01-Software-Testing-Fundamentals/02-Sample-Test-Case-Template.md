# Sample Test Case Template

## Introduction

A **Test Case** is a document that contains a set of inputs, execution steps, expected results, and actual results used to verify whether a software application functions correctly according to the specified requirements.

Test cases help testers execute testing in a structured and organized manner while ensuring that all functionalities of the application are properly validated.

## What is a Test Case?

A **Test Case** is a collection of conditions, test data, execution steps, and expected outcomes that are designed to verify a specific functionality of a software application.

A well-written test case helps testers:

- **Verify application functionality.**
- **Identify defects in the software.**
- **Ensure requirements are met.**
- **Maintain consistency during testing.**
- **Improve software quality.**

## Components of a Test Case

A basic test case generally contains the following fields:

| **Field** | **Description** |
|-----------|-----------------|
| **Test Case ID** | Unique identifier for each test case. |
| **Inputs** | Input values provided during testing. |
| **Expected Output** | The expected result according to the requirement. |
| **Actual Output** | The actual result produced by the application. |
| **Result** | Indicates whether the test case **Passed** or **Failed**. |

## Sample Test Case Template

| **Test Case ID** | **Inputs** | **Expected Output** | **Actual Output** | **Result** |
|------------------|------------|---------------------|-------------------|------------|
| **TI-01** | A = 5<br>B = 10 | 15 | 15 | **Pass** |
| **TI-02** | A = 5<br>B = 10 | 10 | 10 | **Pass** |
| **TI-03** | A = 5<br>B = 0 | 5 | 0 | **Fail** |

## Explanation of the Above Test Cases

### Test Case TI-01

- **Input:** A = 5, B = 10
- **Expected Output:** 15
- **Actual Output:** 15
- **Result:** **Pass**

The application produced the expected result, so the test case is marked as **Pass**.

### Test Case TI-02

- **Input:** A = 5, B = 10
- **Expected Output:** 10
- **Actual Output:** 10
- **Result:** **Pass**

The application behaved as expected for the given requirement.

### Test Case TI-03

- **Input:** A = 5, B = 0
- **Expected Output:** 5
- **Actual Output:** 0
- **Result:** **Fail**

The expected result does not match the actual result. Therefore, this test case is marked as **Fail**, indicating the presence of a defect that should be investigated.

## Why Test Cases are Important

Writing test cases helps to:

- **Ensure complete requirement validation.**
- **Improve testing accuracy.**
- **Reduce the chances of missing functionality.**
- **Simplify defect identification.**
- **Support regression testing.**
- **Maintain testing documentation for future releases.**

## Key Points

- **Every test case should have a unique Test Case ID.**
- **Expected Output is derived from the requirement specification.**
- **Actual Output is obtained after executing the test case.**
- **A test case is marked as Pass only when the Expected Output matches the Actual Output.**
- **If there is any mismatch, the Result is marked as Fail and a defect may be logged.**

## Summary

A **Test Case** is an essential document in Manual Testing that helps verify whether a software application behaves according to its requirements. A properly designed test case improves testing efficiency, ensures application quality, and simplifies defect tracking throughout the software testing process.
