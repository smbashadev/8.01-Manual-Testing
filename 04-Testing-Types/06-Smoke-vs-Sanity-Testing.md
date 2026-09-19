# Smoke Testing vs Sanity Testing

## Introduction

**Smoke Testing** and **Sanity Testing** are two important software testing techniques performed by QA Engineers to verify the stability and functionality of a software application.

Although both are preliminary testing techniques, they differ in their objective, scope, and execution. Understanding the differences between Smoke Testing and Sanity Testing is one of the most commonly asked topics in Manual Testing interviews.

---

## Smoke Testing

### Definition

**Smoke Testing** is a type of testing in which a Test Engineer verifies the **basic and critical functionalities** of a software application to determine whether the build is stable enough for further testing.

Smoke Testing is also known as:

- **Build Verification Testing (BVT)**
- **Build Acceptance Testing (BAT)**
- **Skim Testing**

---

## Sanity Testing

### Definition

**Sanity Testing** is a type of testing in which a Test Engineer verifies the **overall functionality** of a software application after receiving a stable build or after bug fixes have been implemented.

The primary objective of Sanity Testing is to ensure that the modified functionality works correctly and that no major issues are introduced after changes.

---

## Comparison Table

| **Smoke Testing** | **Sanity Testing** |
|-------------------|--------------------|
| Tests the **basic and critical functionalities** of the software. | Tests the **overall functionality** or modified functionality of the software. |
| High-level and **wide** testing. | Deep and **narrow** testing. |
| Performed **before accepting the build**. | Performed **after accepting the build**. |
| Verifies whether the build is stable. | Verifies whether recent changes work correctly. |
| Executed immediately after receiving a new build. | Executed after bug fixes or minor changes. |
| Covers major functionalities only. | Focuses on specific modules or affected functionalities. |
| Determines whether detailed testing can begin. | Determines whether the modified functionality behaves correctly. |
| Usually takes less time. | Usually takes more time than Smoke Testing but less than complete Regression Testing. |

---

## Advantages of Smoke Testing

- **Identifies unstable builds quickly.**
- **Saves testing time and effort.**
- **Prevents testing defective builds.**
- **Improves communication between developers and testers.**
- **Ensures only stable builds proceed for detailed testing.**

---

## Advantages of Sanity Testing

- **Verifies bug fixes quickly.**
- **Ensures modified functionality works correctly.**
- **Reduces unnecessary Regression Testing.**
- **Improves software quality after changes.**
- **Helps detect side effects introduced by recent modifications.**

---

## Real-Time Example

Suppose a company develops an **Online Banking Application**.

### Smoke Testing

After receiving **Build 2.0**, the QA Engineer verifies:

- Application launches successfully.
- Login page works.
- Dashboard loads correctly.
- Logout works.

If these basic functionalities work, the build is accepted for further testing.

---

### Sanity Testing

Later, developers fix a defect in the **Fund Transfer Module**.

The QA Engineer performs Sanity Testing by checking:

- Fund Transfer
- Transaction Confirmation
- Updated Account Balance

Instead of testing the entire application, only the affected functionality is verified.

---

## Smoke Testing Workflow

```text
Receive New Build
        │
        ▼
Smoke Testing
        │
        ▼
Build Stable?
     ┌──┴──┐
     │     │
   Yes      No
    │        │
    ▼        ▼
Detailed   Return Build
Testing    to Developers
```

---

## Sanity Testing Workflow

```text
Bug Fix / Minor Change
          │
          ▼
Receive Updated Build
          │
          ▼
Sanity Testing
          │
          ▼
Functionality Working?
      ┌───┴───┐
      │       │
    Yes       No
     │         │
     ▼         ▼
Continue    Return to
Testing     Developers
```

---

## When to Perform Smoke Testing

Perform Smoke Testing when:

- **A new software build is received.**
- **Critical functionality needs quick verification.**
- **The build must be accepted or rejected.**
- **Before detailed testing begins.**

---

## When to Perform Sanity Testing

Perform Sanity Testing when:

- **A bug has been fixed.**
- **Minor functionality has been modified.**
- **Regression Testing is unnecessary.**
- **The build has already passed Smoke Testing.**

---

## Frequently Asked Interview Questions

### 1. What is the main purpose of Smoke Testing?

To verify whether the software build is stable enough for detailed testing.

---

### 2. What is the main purpose of Sanity Testing?

To verify that recently modified or fixed functionality works correctly.

---

### 3. Which testing is performed first?

**Smoke Testing** is performed before **Sanity Testing**.

---

### 4. Is Smoke Testing broad or narrow?

**Smoke Testing is broad and high-level.**

---

### 5. Is Sanity Testing broad or narrow?

**Sanity Testing is narrow and deep.**

---

### 6. Is Sanity Testing a part of Regression Testing?

Yes. **Sanity Testing is considered a subset of Regression Testing** because it verifies specific changes after bug fixes.

---

## Key Points

- **Smoke Testing validates build stability.**
- **Sanity Testing validates recent changes or bug fixes.**
- **Smoke Testing is broad and shallow.**
- **Sanity Testing is narrow and focused.**
- **Smoke Testing is performed before accepting a build.**
- **Sanity Testing is performed after the build is accepted.**
- **Both testing techniques save time by avoiding unnecessary detailed testing.**

---

## Summary

**Smoke Testing** and **Sanity Testing** are preliminary software testing techniques that help ensure software quality before detailed testing. Smoke Testing focuses on verifying the stability of a newly received build by testing basic and critical functionalities, whereas Sanity Testing verifies the correctness of recently modified or fixed functionalities after the build has been accepted. Understanding the differences between these two testing techniques is essential for Software Test Engineers and is one of the most frequently asked topics in Manual Testing interviews.
