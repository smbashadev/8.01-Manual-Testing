# Smoke Testing

## Introduction

**Smoke Testing** is one of the initial software testing techniques performed after a new software build is received from the development team. Its primary objective is to verify whether the application's basic and critical functionalities are working correctly before performing detailed testing.

If the critical functionalities fail during Smoke Testing, the build is rejected and returned to the development team for fixing. This helps save testing time and prevents unnecessary execution of detailed test cases on an unstable build.

Smoke Testing is generally the first level of testing performed after every new software build.

---

## Definition

**Smoke Testing**, also known as **Build Verification Testing (BVT)**, **Build Acceptance Testing (BAT)**, or **Skim Testing**, is a type of testing in which a Test Engineer verifies the **basic and critical functionalities** of a software application to ensure that the build is stable enough for further testing.

The purpose of Smoke Testing is to determine whether the software build is suitable for detailed functional testing.

---

Smoke Testing Coverage Timeline

During Smoke Testing, the Test Engineer verifies only the basic and critical functionalities of the application instead of executing every test case. This initial verification helps determine whether the received software build is stable enough for detailed testing.

The following diagram illustrates that Smoke Testing quickly validates the most important functionalities from both Black Box Testing and White Box Testing during the initial days after receiving a new build.

Black Box Testing                      Smoke Testing                      White Box Testing

Functional        ─┐                                            ┌─ Statement
Integration       ─┤                                            ├─ Path
System            ─┤──────► Verify Basic & Critical ◄───────────┤─ Loop
Acceptance        ─┘          Functionalities                  └─ Conditional

                     Day 1    Day 2    Day 3    Day 4
                        │        │        │        │
                        └──────── Smoke Testing ────────┘

Figure: Smoke Testing Coverage Timeline showing early verification of critical Black Box and White Box testing areas.

## Other Names of Smoke Testing

Smoke Testing is also known as:

- **Build Verification Testing (BVT)**
- **Build Acceptance Testing (BAT)**
- **Skim Testing**

All these terms refer to the same testing process.

---

## Purpose of Smoke Testing

The main objectives of Smoke Testing are:

- **Verify that the software build is stable.**
- **Ensure critical functionalities are working correctly.**
- **Identify major defects at an early stage.**
- **Reduce testing effort by rejecting unstable builds.**
- **Save testing time and resources.**
- **Confirm that the build is ready for detailed testing.**

---

## Build Verification Testing (BVT)

### Definition

**Build Verification Testing (BVT)** is another name for **Smoke Testing**.

It verifies whether the newly received software build is stable and whether its core functionalities work correctly before detailed testing begins.

### Objectives

- Verify build stability.
- Confirm successful deployment.
- Validate basic functionality.
- Decide whether to continue or reject testing.

---

## Build Acceptance Testing (BAT)

### Definition

**Build Acceptance Testing (BAT)** is the process of accepting or rejecting a software build after verifying its critical functionalities.

If the Smoke Test passes, the build is accepted.

If the Smoke Test fails, the build is rejected and sent back to the development team.

### Build Status

**Build Accepted**

- Basic features are working.
- Testing can continue.

**Build Rejected**

- Critical functionality is not working.
- Build is returned to developers.

---

## Skim Testing

### Definition

**Skim Testing** is another commonly used name for **Smoke Testing**.

Instead of testing every feature in detail, only the important and high-priority functionalities are checked quickly to determine whether the software is stable.

---

## Smoke Testing Workflow

```text
Developer
    │
    ▼
Software Build
    │
    ▼
Smoke Testing
    │
    ▼
Is Build Stable?
    │
 ┌──┴──┐
 │     │
Yes    No
 │      │
 ▼      ▼
Detailed   Return Build
Testing    to Developers
```

---

## Characteristics of Smoke Testing

- **Performed on every new software build.**
- **Tests only critical functionalities.**
- **Quick and lightweight testing process.**
- **Performed before Functional Testing.**
- **Helps determine build stability.**
- **Reduces unnecessary testing effort.**
- **Usually performed manually or using automation tools.**

---

## Advantages of Smoke Testing

- **Detects major defects early.**
- **Saves testing time.**
- **Improves software quality.**
- **Prevents testing unstable builds.**
- **Reduces project risk.**
- **Improves communication between developers and testers.**
- **Ensures only stable builds proceed for further testing.**

---

## Disadvantages of Smoke Testing

- **Does not verify all functionalities.**
- **Cannot identify detailed functional defects.**
- **Only provides confidence in build stability.**
- **Requires additional testing after completion.**

---

## Real-Time Example

Suppose a company develops an **Online Banking Application**.

A new software build is delivered to the QA team.

Before executing hundreds of functional test cases, the Test Engineer verifies only the critical features:

- Application launches successfully.
- Login functionality works.
- Dashboard opens correctly.
- Balance enquiry page loads.
- Logout functionality works.

If these basic functionalities work correctly, the build is accepted and detailed testing begins.

If the Login page itself fails, the build is rejected immediately and returned to the developers.

This process is called **Smoke Testing**.

---

## Difference Between Smoke Testing and Detailed Functional Testing

| **Smoke Testing** | **Detailed Functional Testing** |
|-------------------|---------------------------------|
| Tests basic functionalities. | Tests every functionality in detail. |
| Performed first. | Performed after Smoke Testing. |
| Verifies build stability. | Verifies business requirements. |
| Takes less time. | Takes more time. |
| Determines whether testing should continue. | Finds functional defects throughout the application. |

---

## Frequently Asked Interview Questions

### 1. What is Smoke Testing?

Smoke Testing is a testing technique used to verify the basic and critical functionalities of a software build before detailed testing begins.

---

### 2. What are the other names for Smoke Testing?

- Build Verification Testing (BVT)
- Build Acceptance Testing (BAT)
- Skim Testing

---

### 3. Why is Smoke Testing performed?

To verify whether the software build is stable enough for further testing.

---

### 4. Who performs Smoke Testing?

**Software Test Engineers (QA Engineers).**

---

### 5. When is Smoke Testing performed?

Immediately after receiving every new software build from the development team.

---

## Key Points

- **Smoke Testing verifies basic and critical functionalities.**
- **Performed on every new software build.**
- **Also known as BVT, BAT, and Skim Testing.**
- **Helps determine build stability.**
- **Prevents testing unstable software builds.**
- **Executed before detailed functional testing.**

---

## Summary

**Smoke Testing** is a quick verification process performed after receiving a new software build. It focuses on validating the application's basic and critical functionalities to determine whether the build is stable enough for detailed testing. Also known as **Build Verification Testing (BVT)**, **Build Acceptance Testing (BAT)**, and **Skim Testing**, it helps save testing effort by rejecting unstable builds early and ensuring that only reliable software proceeds to the next phase of testing.
