# Retesting

## Introduction

During software testing, defects are identified and reported to the development team. After developers fix these defects, the corrected build is sent back to the QA team for verification.

The QA team executes the same failed test cases again to confirm whether the reported defect has been fixed successfully. This process is known as **Retesting**.

Unlike Regression Testing, which checks whether existing functionality is affected by changes, Retesting focuses only on verifying the specific defect that was previously reported.

---

## Definition

**Retesting** is the process of **testing the software again by re-executing the failed test cases on the same build** after the reported defects have been fixed.

Normally, Retesting is performed to:

- **Confirm that the reported defect has been fixed.**
- **Verify the corrected functionality.**
- **Ensure the application behaves according to the expected requirements.**

---

## Objectives of Retesting

Retesting is performed to:

- **Verify defect fixes.**
- **Confirm expected functionality.**
- **Ensure previously failed test cases now pass.**
- **Prevent reopening of already fixed defects.**
- **Improve software quality before release.**

---

## Retesting Workflow

The following workflow illustrates the Retesting process.

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
Functional Testing
     │
     ▼
Defect Found
     │
     ▼
Bug Reported
     │
     ▼
Developer Fixes Bug
     │
     ▼
Same Build Received
     │
     ▼
Retesting
     │
     ▼
Bug Fixed?
   ┌──┴──┐
   │     │
 Yes     No
  │       │
  ▼       ▼
Close   Reopen
Defect  Defect
```

---

## Sample Test Case Template

Suppose a defect is identified in the **Login Module** of a Gmail Application.

### Login Screen

```text
----------------------------
        Gmail Login
----------------------------

Username : ___________

Password : ___________

        [ Login ]
----------------------------
```

---

### Sample Test Cases

| **Test Case ID** | **Inputs** | **Procedure** | **Expected Output** | **Actual Output** | **Result** |
|------------------|------------|---------------|---------------------|-------------------|------------|
| **FT-01** | UN = Kod<br>PW = 123 | Enter Username and Password, then click **Login**. | Successfully login and Inbox should be displayed. | Password is visible in the Password field, which is a security issue. | **Fail** |
| **FT-02** | UN = NET<br>PW = 789 | Enter Username and Password, then click **Login**. | Successfully login and Inbox should be displayed. | Password is visible in the Password field, which is a security issue. | **Fail** |
| **FT-03** | UN = DOT<br>PW = 456 | Enter Username and Password, then click **Login**. | Successfully login and Inbox should be displayed. | Password is visible in the Password field, which is a security issue. | **Fail** |
| **FT-04** | UN = KodNest<br>PW = 213121 | Enter Username and Password, then click **Login**. | Successfully login and Inbox should be displayed. | Password is visible in the Password field, which is a security issue. | **Fail** |

---

## Retesting Scenario

After identifying the above defect, the QA Engineer reports it to the development team.

The developers modify the Login page so that the password is displayed as masked characters (**●●●●●** or ******) instead of plain text.

The same build is then returned to the QA team.

The QA Engineer executes only the failed Login test cases again.

If the password is now properly masked, the defect is marked as **Fixed** and **Closed**.

Otherwise, the defect is **Reopened** and sent back to the developer.

---

## Characteristics of Retesting

- **Performed after bug fixing.**
- **Only failed test cases are executed.**
- **Performed on the same software build.**
- **Confirms whether defects are fixed.**
- **Focused on specific functionality.**
- **Usually performed by QA Engineers.**

---

## Difference Between Retesting and Regression Testing

| **Retesting** | **Regression Testing** |
|----------------|------------------------|
| Verifies previously failed test cases. | Verifies existing functionalities after changes. |
| Performed on the same build after bug fixing. | Performed on a new or modified build. |
| Focuses only on the reported defect. | Focuses on affected and existing functionalities. |
| Objective is to verify bug fixes. | Objective is to ensure no new defects are introduced. |
| Executes failed test cases only. | Executes previously passed and selected test cases. |

---

## Advantages of Retesting

- **Confirms defect resolution.**
- **Ensures software quality.**
- **Prevents reopening of resolved defects.**
- **Improves customer confidence.**
- **Requires fewer test cases compared to Regression Testing.**

---

## Disadvantages of Retesting

- **Focuses only on reported defects.**
- **Does not verify the impact on other modules.**
- **Usually needs Regression Testing after completion.**

---

## Real-Time Example

Consider an **Online Banking Application**.

A tester reports that the **Login Password** is displayed in plain text instead of masked characters.

The defect is assigned to the developer.

The developer fixes the issue and provides the updated build.

The QA Engineer executes only the Login test cases again.

The password is now displayed as:

```text
Password : ********
```

The Login page functions correctly.

The defect is marked as **Closed**.

This process is called **Retesting**.

---

## Frequently Asked Interview Questions

### 1. What is Retesting?

Retesting is the process of re-executing failed test cases on the same build after the reported defects have been fixed.

---

### 2. Why is Retesting performed?

To verify whether the reported defect has been fixed successfully.

---

### 3. Is Retesting performed on the same build or a new build?

**Retesting is generally performed on the same build after bug fixes.**

---

### 4. Which test cases are executed during Retesting?

Only the **previously failed test cases**.

---

### 5. What is the main difference between Retesting and Regression Testing?

Retesting verifies the fixed defect, whereas Regression Testing verifies that existing functionalities continue to work correctly after changes.

---

## Key Points

- **Retesting verifies defect fixes.**
- **Only failed test cases are executed.**
- **Performed after bug fixing.**
- **Executed on the same build.**
- **Confirms expected functionality.**
- **Often followed by Regression Testing if required.**

---

## Summary

**Retesting** is a software testing technique performed after developers fix reported defects. It involves re-executing only the previously failed test cases on the same build to confirm that the defect has been resolved successfully. Retesting helps ensure software quality, validates bug fixes, and provides confidence that the corrected functionality behaves according to the specified requirements before the software is released.
