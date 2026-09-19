# Test Case

## Introduction

A **Test Case** is one of the most important documents in Software Testing. It provides a systematic way to verify whether a software application behaves according to the specified requirements.

A well-written Test Case contains all possible scenarios, including valid and invalid inputs, expected outputs, execution steps, and test results. It helps Test Engineers perform testing consistently and ensures complete requirement coverage.

---

## Definition

A **Test Case** is a document containing all the possible test scenarios.

A Test Case is a collection of **inputs** and **expected outputs**. Test Cases are written after understanding the requirements specified in the **Customer Requirement Specification (CRS)**, **Software Requirement Specification (SRS)**, or **Functional Requirement Specification (FRS)** documents.

---

## Objectives of a Test Case

Test Cases are written to:

- **Verify software functionality.**
- **Ensure requirement coverage.**
- **Identify software defects.**
- **Maintain consistency during testing.**
- **Provide proper documentation for testing activities.**
- **Improve software quality.**

---

## Standard Test Case Template

A standard Test Case generally consists of the following columns.

| **Column** | **Description** |
|------------|-----------------|
| **Test Case ID** | Unique identifier for the Test Case. |
| **Project Name** | Name of the software project. |
| **Module Name** | Module being tested. |
| **Requirement Number** | Requirement reference number from CRS/SRS/FRS. |
| **Pre-Requisites / Pre-Conditions** | Conditions that must be satisfied before executing the Test Case. |
| **Inputs / Test Data** | Input values required for execution. |
| **Procedure / Test Case Description** | Step-by-step instructions for executing the Test Case. |
| **Expected Output** | Expected behavior of the application. |
| **Actual Output** | Actual result obtained after execution. |
| **Status / Result** | Pass or Fail status. |
| **Defect Number / Ticket Number** | Bug ID generated if the Test Case fails. |
| **Severity** | Impact of the defect on the application. |
| **Priority** | Urgency of fixing the defect. |

---

## Sample Test Case Template

| Test Case ID | Project Name | Module Name | Requirement Number | Pre-Requisites | Inputs / Test Data | Procedure / Test Case Description | Expected Output | Actual Output | Status | Defect No / Ticket No | Severity | Priority |
|---------------|--------------|-------------|--------------------|----------------|--------------------|-----------------------------------|-----------------|---------------|--------|-----------------------|----------|----------|
| TC-001 | Online Banking | Login | REQ-101 | Application should be running | Username: admin<br>Password: admin123 | Enter valid Username and Password and click **Login** | Login should be successful and Dashboard should be displayed | Same as Expected | Pass | NA | NA | High |

---

## Explanation of Test Case Columns

### Test Case ID

A unique identification number assigned to every Test Case.

Example:

```text
TC-001
TC-002
TC-003
```

---

### Project Name

The name of the software application being tested.

Example:

```text
Online Banking System
Student Management System
E-Commerce Application
```

---

### Module Name

The specific module on which testing is performed.

Example:

- Login
- Registration
- Payment
- Fund Transfer
- Shopping Cart

---

### Requirement Number

The reference number corresponding to the requirement in the CRS, SRS, or FRS document.

Example:

```text
REQ-101
REQ-205
REQ-310
```

---

### Pre-Requisites / Pre-Conditions

Conditions that must be satisfied before executing the Test Case.

Examples:

- Application should be running.
- User should be registered.
- Database should be connected.
- Internet connection should be available.

---

### Inputs / Test Data

The data used for executing the Test Case.

Example:

```text
Username : admin
Password : admin123
```

---

### Procedure / Test Case Description

The sequence of steps to execute the Test Case.

Example:

1. Launch the application.
2. Enter Username.
3. Enter Password.
4. Click Login.
5. Observe the result.

---

### Expected Output

The expected behavior of the application according to the requirement.

Example:

```text
User should successfully log in and Dashboard should be displayed.
```

---

### Actual Output

The actual result observed after executing the Test Case.

Example:

```text
Dashboard displayed successfully.
```

---

### Status / Result

Indicates whether the Test Case passed or failed.

Possible values:

- Pass
- Fail
- Blocked
- Not Executed

---

### Defect Number / Ticket Number

If the Test Case fails, a defect or ticket number is assigned.

Example:

```text
BUG-101
JIRA-205
MANTIS-89
```

---

### Severity

Severity indicates the impact of the defect on the software.

Common severity levels include:

- Critical
- High
- Medium
- Low

---

### Priority

Priority indicates how quickly the defect should be fixed.

Common priority levels include:

- High
- Medium
- Low

---

## Steps Involved in Writing a Test Case

The process of writing a Test Case generally involves the following steps.

### Step 1 – Requirement Study

Study and understand the requirements provided in the CRS, SRS, or FRS documents.

---

### Step 2 – Identify All Possible Scenarios

Identify every possible positive and negative scenario that a user may perform.

Examples include:

- Valid input
- Invalid input
- Boundary values
- Blank fields
- Special characters

---

### Step 3 – Write the Test Case Using Test Case Design Techniques

Prepare Test Cases using suitable Test Case Design Techniques such as:

- Boundary Value Analysis (BVA)
- Equivalence Class Partitioning (ECP)
- Error Guessing

---

### Step 4 – Review the Test Case

The prepared Test Cases are reviewed by another Test Engineer having an equivalent designation to identify mistakes or missing scenarios.

---

### Step 5 – Test Case Approval

After review, the Test Lead or QA Manager approves the Test Cases for execution.

---

### Step 6 – Store the Test Case

Approved Test Cases are stored in a **Test Case Repository** or a **Shared Repository** so that the Testing Team can access and reuse them whenever required.

---

## Test Case Workflow

```text
Requirement Study
        │
        ▼
Identify Test Scenarios
        │
        ▼
Design Test Cases
        │
        ▼
Review Test Cases
        │
        ▼
Approval
        │
        ▼
Store in Test Case Repository
        │
        ▼
Execute Test Cases
```

---

## Characteristics of a Good Test Case

A good Test Case should be:

- **Clear**
- **Simple**
- **Accurate**
- **Reusable**
- **Traceable**
- **Complete**
- **Easy to Execute**
- **Easy to Maintain**

---

## Advantages of Writing Test Cases

- **Ensures complete requirement coverage.**
- **Reduces testing errors.**
- **Improves testing consistency.**
- **Makes defect identification easier.**
- **Supports future regression testing.**
- **Provides proper testing documentation.**

---

## Real-Time Example

Consider an **Online Banking Application**.

Requirement:

"The user should be able to log in using a valid Username and Password."

The Test Engineer prepares multiple Test Cases such as:

- Valid Username and Valid Password
- Invalid Username
- Invalid Password
- Empty Username
- Empty Password
- SQL Injection attempt
- Maximum length validation

These Test Cases help verify the Login functionality completely.

---

## Frequently Asked Interview Questions

### 1. What is a Test Case?

A Test Case is a document containing all possible testing scenarios, inputs, expected outputs, and execution steps used to verify software functionality.

---

### 2. Who writes Test Cases?

Generally, **Software Test Engineers** write Test Cases.

---

### 3. What documents are referred to while writing Test Cases?

- Customer Requirement Specification (CRS)
- Software Requirement Specification (SRS)
- Functional Requirement Specification (FRS)

---

### 4. What are the major columns in a Test Case?

- Test Case ID
- Project Name
- Module Name
- Requirement Number
- Pre-Requisites
- Inputs
- Procedure
- Expected Output
- Actual Output
- Status
- Defect Number
- Severity
- Priority

---

### 5. What is the purpose of a Test Case Repository?

A Test Case Repository stores approved Test Cases for execution, maintenance, and future reuse.

---

## Key Points

- **Test Cases are written after Requirement Study.**
- **They contain all possible testing scenarios.**
- **A standard Test Case follows a predefined template.**
- **Review and approval are mandatory before execution.**
- **Approved Test Cases are stored in a Test Case Repository.**
- **Well-written Test Cases improve software quality and testing efficiency.**

---

## Summary

A **Test Case** is a structured document that describes how a particular functionality should be tested. It includes inputs, execution steps, expected results, actual results, defect details, severity, and priority. Test Cases are prepared after studying the project requirements and following a systematic process that includes requirement analysis, scenario identification, Test Case design, review, approval, and storage. Properly designed Test Cases ensure complete requirement coverage, improve testing quality, and contribute significantly to successful software delivery.
