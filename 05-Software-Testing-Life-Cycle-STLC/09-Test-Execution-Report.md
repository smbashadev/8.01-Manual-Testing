# Test Execution Report

## Introduction

The **Test Execution Report (TER)** is the final deliverable of the Software Testing Life Cycle (STLC). After all planned Test Cases are executed, the Testing Team prepares a report summarizing the overall testing progress and results.

The Test Execution Report provides stakeholders with a clear understanding of the software quality, testing coverage, defects identified, and the readiness of the application for release.

It serves as an important document for project managers, developers, clients, and quality assurance teams when making release decisions.

---

## Definition

**Test Execution Report** is a report generated once the execution of Test Cases is completed.

The Test Execution Report contains the status of the Test Execution, including the total number of Test Cases, executed Test Cases, passed Test Cases, failed Test Cases, and their corresponding percentages.

---

## Objectives of Test Execution Report

The Test Execution Report is prepared to:

- **Summarize the testing activities performed.**
- **Provide the execution status of Test Cases.**
- **Measure testing progress.**
- **Report the number of passed and failed Test Cases.**
- **Support release decisions.**
- **Provide testing metrics to stakeholders.**

---

## Test Execution Report Template

| **Module Name** | **Total Test Cases** | **Executed Test Cases** | **Passed** | **Failed** | **Pass %** | **Fail %** |
|-----------------|---------------------:|------------------------:|------------:|------------:|-----------:|-----------:|
| Login | 400 | 200 | 100 | 100 | 50% | 50% |
| Inbox | 200 | 100 | 50 | 50 | 50% | 50% |
| Compose | 300 | 300 | 150 | 150 | 50% | 50% |
| Sent Messages | 100 | 100 | 70 | 30 | 70% | 30% |

---

## Components of a Test Execution Report

A standard Test Execution Report generally contains the following information.

### Project Information

- Project Name
- Module Name
- Build Number
- Version Number
- Test Environment
- Execution Date

---

### Test Case Summary

The report includes:

- Total Test Cases
- Executed Test Cases
- Passed Test Cases
- Failed Test Cases
- Blocked Test Cases (if any)
- Not Executed Test Cases (if any)

---

### Defect Summary

The report also contains:

- Total Defects Reported
- Critical Defects
- Major Defects
- Minor Defects
- Closed Defects
- Reopened Defects

---

### Execution Statistics

The report provides statistics such as:

- Pass Percentage
- Fail Percentage
- Execution Percentage
- Pending Test Cases

---

## Test Execution Workflow

```text
Execute Test Cases
        │
        ▼
Record Results
        │
        ▼
Update Pass / Fail Status
        │
        ▼
Prepare Execution Statistics
        │
        ▼
Generate Test Execution Report
        │
        ▼
Share with Stakeholders
```

---

## Pass Percentage Formula

```text
Pass Percentage

=

(Number of Passed Test Cases / Number of Executed Test Cases) × 100
```

### Example

```text
Executed Test Cases = 200

Passed Test Cases = 150

Pass %

=

(150 / 200) × 100

=

75%
```

---

## Fail Percentage Formula

```text
Fail Percentage

=

(Number of Failed Test Cases / Number of Executed Test Cases) × 100
```

### Example

```text
Executed Test Cases = 200

Failed Test Cases = 50

Fail %

=

(50 / 200) × 100

=

25%
```

---

## Daily Test Execution Report

In most real-time projects, the **Junior Test Engineer** prepares and updates the Test Execution Report **daily**.

The report helps the Test Lead and Project Manager monitor:

- Daily testing progress.
- Number of executed Test Cases.
- Pending Test Cases.
- Newly identified defects.
- Overall testing status.

---

## Test Execution Schedule Example

Example project schedule:

```text
Functional Testing      : 30 Days

Regression Testing      : 15 Days

Future Testing Activities : 10 Days

Buffer Time             : 5 Days

--------------------------------------

Total Project Duration  : 60 Days

                       = 2 Months
```

---

## Advantages of Test Execution Report

- **Provides complete testing status.**
- **Helps management monitor project progress.**
- **Supports software release decisions.**
- **Tracks execution performance.**
- **Improves communication among stakeholders.**
- **Acts as historical project documentation.**

---

## Real-Time Example

Consider an **Online Banking Application**.

The Login Module contains **250 Test Cases**.

After execution:

- Executed Test Cases: **250**
- Passed Test Cases: **240**
- Failed Test Cases: **10**

The Test Execution Report summarizes these results and is shared with the Project Manager and QA Manager.

If all critical defects are fixed and the pass percentage meets the project standards, the application can be recommended for release.

---

## Frequently Asked Interview Questions

### 1. What is a Test Execution Report?

A Test Execution Report is a document generated after Test Case execution that summarizes the execution results and overall testing status.

---

### 2. Who prepares the Test Execution Report?

Generally, the **Junior Test Engineer** prepares and updates the Test Execution Report on a daily basis.

---

### 3. What information is included in a Test Execution Report?

- Module Name
- Total Test Cases
- Executed Test Cases
- Passed Test Cases
- Failed Test Cases
- Pass Percentage
- Fail Percentage
- Defect Summary

---

### 4. Why is a Test Execution Report important?

It helps stakeholders understand testing progress, software quality, defect status, and release readiness.

---

### 5. Which phase is the final phase of STLC?

**Test Execution Report** is the final phase of the Software Testing Life Cycle (STLC).

---

## Key Points

- **The Test Execution Report is the final deliverable of STLC.**
- **It summarizes the overall Test Execution results.**
- **It includes Pass %, Fail %, and execution statistics.**
- **It is generally updated daily by the Junior Test Engineer.**
- **The report helps stakeholders decide whether the software is ready for release.**

---

## Summary

The **Test Execution Report (TER)** is the final document generated during the Software Testing Life Cycle (STLC) after executing all planned Test Cases. It summarizes the execution status, including the total number of Test Cases, executed, passed, and failed Test Cases, along with execution statistics and defect information. Prepared and updated regularly by the Testing Team, the Test Execution Report provides valuable insights into software quality, testing progress, and release readiness, enabling stakeholders to make informed project and deployment decisions.
