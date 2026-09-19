# Error Masking

## Introduction

**Error Masking** is a software testing concept in which an existing error or defect remains hidden because another defect or condition prevents it from being detected during testing.

When error masking occurs, testers may not identify the actual defect, making it difficult to evaluate the software correctly.

## Definition

**Error Masking** is the process of hiding the errors present in the **test case template** or software application, making them difficult to detect during the testing process.

**Error Masking** started in the **year 1960**.

## How Error Masking Occurs

Error masking generally occurs when:

- **One defect hides another defect.**
- **The application does not reach the section where the actual defect exists.**
- **Incorrect input or unexpected behavior prevents another error from being observed.**
- **A previously occurring defect blocks the execution of subsequent functionalities.**

As a result, the tester may identify only the visible defect while the hidden defect remains undiscovered.

## Real-Time Example

Consider a **Login Page** with the following issues:

- The **Login** button is disabled due to a user interface defect.
- The password validation logic also contains a defect.

Since the **Login** button cannot be clicked, the password validation logic is never executed.

In this situation, the password validation defect remains hidden because the first defect prevents it from being detected. This is an example of **Error Masking**.

## Why Error Masking is a Problem

Error masking can lead to several challenges:

- **Hidden defects remain undetected.**
- **Testing results become inaccurate.**
- **Software quality may decrease.**
- **Additional defects may appear after fixing the visible issue.**
- **It increases the overall testing effort and time.**

## Key Points

- **Error Masking hides existing defects during software testing.**
- **It usually occurs when one defect prevents another defect from being detected.**
- **The concept of Error Masking was introduced in 1960.**
- **Independent and thorough testing helps reduce Error Masking.**
- **Proper test case design can minimize the chances of hidden defects.**

## Summary

**Error Masking** is a testing concept where one defect conceals another defect, preventing it from being identified during testing. Understanding Error Masking helps testers design better test cases and perform more effective testing to uncover hidden defects before software is released.
