# Test Execution

## Introduction

After Test Cases are designed, reviewed, and approved, the next phase in the Software Testing Life Cycle (STLC) is **Test Execution**. During this phase, the Test Engineer executes the prepared Test Cases on the software application and verifies whether the application behaves according to the expected requirements.

The actual results obtained during execution are compared with the expected results. If any difference is observed, it is reported as a defect.

Test Execution is one of the most important phases because it determines the quality and reliability of the software.

---

## Definition

**Test Execution** is the process of executing the prepared Test Cases once the software is completely built.

Once the Test Cases are executed, the remaining columns in the Test Case Template are filled based on the actual execution results.

---

## Objectives of Test Execution

Test Execution is performed to:

- **Verify that the software meets the specified requirements.**
- **Compare actual results with expected results.**
- **Identify defects in the application.**
- **Validate software functionality.**
- **Record execution results for future reference.**
- **Ensure software quality before release.**

---

## Prerequisites for Test Execution

Before executing Test Cases, the following conditions should be satisfied:

- Requirements are finalized.
- Test Cases are prepared and approved.
- Testing Environment is ready.
- Test Data is available.
- Software Build is stable.
- Test Plan is approved.

---

## Test Execution Process

The Test Execution process generally consists of the following steps.

### Step 1 – Receive the Software Build

The Development Team delivers the completed software build to the Testing Team.

---

### Step 2 – Verify the Testing Environment

The Test Engineer verifies that the required hardware, software, database, browsers, and network are available.

---

### Step 3 – Execute Test Cases

The Test Engineer executes the prepared Test Cases according to the Test Plan.

---

### Step 4 – Compare Results

The **Actual Output** is compared with the **Expected Output**.

---

### Step 5 – Update Test Case Status

Based on the execution result, the Test Case status is updated.

Possible statuses include:

- Pass
- Fail
- Blocked
- Not Executed

---

### Step 6 – Report Defects

If the Actual Output does not match the Expected Output, a defect is logged into the defect tracking tool.

---

### Step 7 – Prepare Execution Report

After all Test Cases are executed, the Test Execution Report is prepared.

---

## Test Execution Workflow

```text
Receive Software Build
          │
          ▼
Verify Testing Environment
          │
          ▼
Execute Test Cases
          │
          ▼
Compare Expected Output
with Actual Output
          │
     ┌────┴────┐
     │         │
   Match    Not Match
     │         │
     ▼         ▼
   Pass     Report Defect
     │         │
     └────┬────┘
          ▼
Update Test Case Status
          │
          ▼
Prepare Test Execution Report
```

---

## Test Case Columns Updated During Execution

After executing a Test Case, the following columns are updated.

| **Column** | **Purpose** |
|------------|-------------|
| Actual Output | Records the actual behavior of the application. |
| Status / Result | Indicates Pass, Fail, Blocked, or Not Executed. |
| Defect Number / Ticket Number | Stores the defect ID if the Test Case fails. |
| Severity | Specifies the impact of the defect. |
| Priority | Specifies how urgently the defect should be fixed. |

---

## Sample Test Case Execution

| Test Case ID | Expected Output | Actual Output | Status | Defect No | Severity | Priority |
|---------------|-----------------|---------------|--------|------------|----------|----------|
| TC-001 | Login successful and Dashboard displayed | Dashboard displayed successfully | Pass | NA | NA | High |
| TC-002 | Error message for invalid password | Application crashes | Fail | BUG-101 | Critical | High |

---

## Possible Test Execution Status

### Pass

The Actual Output matches the Expected Output.

---

### Fail

The Actual Output does not match the Expected Output.

A defect is reported.

---

### Blocked

The Test Case cannot be executed due to dependency issues.

Example:

- Server unavailable
- Database connection failure
- Environment issue

---

### Not Executed

The Test Case has not yet been executed.

---

## Deliverables of Test Execution

The Test Execution phase produces:

- Updated Test Cases
- Defect Reports
- Execution Logs
- Execution Status Report
- Test Execution Report

---

## Advantages of Test Execution

- **Validates software functionality.**
- **Identifies software defects.**
- **Ensures requirement compliance.**
- **Provides execution history.**
- **Improves software quality.**
- **Supports release decisions.**

---

## Real-Time Example

Consider an **Online Banking Application**.

The Login module contains ten Test Cases.

The Test Engineer executes all ten Test Cases.

Results:

- 8 Test Cases passed.
- 2 Test Cases failed.

The failed Test Cases are logged in JIRA with appropriate severity and priority.

After the defects are fixed, the Test Engineer performs Retesting and Regression Testing before updating the Test Execution Report.

---

## Frequently Asked Interview Questions

### 1. What is Test Execution?

Test Execution is the process of executing prepared Test Cases on the software application and comparing Actual Output with Expected Output.

---

### 2. Which STLC phase follows Test Case Design?

**Test Execution.**

---

### 3. What happens if the Actual Output differs from the Expected Output?

A defect is reported and assigned a Defect Number or Ticket Number.

---

### 4. Which Test Case columns are updated during execution?

- Actual Output
- Status / Result
- Defect Number
- Severity
- Priority

---

### 5. What are the possible Test Execution statuses?

- Pass
- Fail
- Blocked
- Not Executed

---

## Key Points

- **Test Execution is the phase where approved Test Cases are executed.**
- **Actual Output is compared with Expected Output.**
- **Defects are reported whenever mismatches are found.**
- **Execution results are recorded in the Test Case Template.**
- **Test Execution helps determine software quality before release.**

---

## Summary

**Test Execution** is the phase of the Software Testing Life Cycle in which approved Test Cases are executed on the completed software application. During execution, the Test Engineer compares the Actual Output with the Expected Output, updates the execution status, and reports any defects found. The results of Test Execution are documented in Test Cases and Test Execution Reports, providing valuable information about the application's quality and readiness for release.
