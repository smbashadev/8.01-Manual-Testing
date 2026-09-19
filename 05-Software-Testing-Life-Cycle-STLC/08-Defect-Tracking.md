# Defect Tracking

## Introduction

During Test Execution, if the Actual Output does not match the Expected Output, it indicates the presence of a defect. These defects must be recorded, monitored, assigned, fixed, verified, and finally closed.

**Defect Tracking** is the process that helps the Testing Team and Development Team communicate effectively about defects. It ensures that every reported defect is tracked until it is resolved.

Defect Tracking is one of the most important phases of the Software Testing Life Cycle (STLC).

---

## Definition

**Defect Tracking** is the process of identifying, isolating, recording, tracking, and managing software defects.

Once the defects are identified, they must be reported to the Development Team so that they can be fixed.

---

## Objectives of Defect Tracking

Defect Tracking is performed to:

- **Identify software defects.**
- **Record complete defect information.**
- **Assign defects to developers.**
- **Monitor defect status.**
- **Verify defect fixes.**
- **Ensure defects are properly closed.**
- **Improve software quality.**

---

## Ways of Reporting Defects

Once defects are identified, they can be reported using any of the following methods.

### 1. Email Communication

The Test Engineer writes an email to the Developer explaining:

- Defect Summary
- Steps to Reproduce
- Expected Result
- Actual Result
- Severity
- Screenshots
- Supporting Documents

---

### 2. Defect Tracking Tools

In real-time projects, defects are reported using Defect Tracking Tools.

Some commonly used tools are:

- **JIRA**
- **Bugzilla**
- **Mantis**

These tools help monitor the complete lifecycle of every defect.

---

## Standard Defect Report Template

| **Field** | **Description** |
|------------|-----------------|
| **Defect Number** | Unique defect identification number. |
| **Defect Summary** | Short description of the defect. |
| **Steps for Reproducibility** | Steps to reproduce the defect. |
| **Submitted Author** | Name of the Test Engineer who reported the defect. |
| **Submission Date** | Date on which the defect was reported. |
| **Version Number** | Software version where the defect was found. |
| **Build Number** | Build number under testing. |
| **Assigned To** | Developer responsible for fixing the defect. |
| **Severity** | Impact of the defect. |
| **Screenshot** | Screenshot showing the defect. |

---

## Sample Defect Report

| Defect No | Defect Summary | Steps for Reproducibility | Submitted Author | Submission Date | Version No | Build No | Assigned To | Severity | Screenshot |
|------------|----------------|---------------------------|------------------|-----------------|------------|-----------|-------------|----------|------------|
| 01 | Password is visible in the Password field of the Gmail Login Page | Enter **2222222** in the Password field of the Gmail Login Page | Basha | 06/11/2023 | 02 | 01 | Deep | Major | Attached |

---

## Defect Lifecycle

A reported defect passes through several stages before it is finally closed.

```text
New
 │
 ▼
Assigned
 │
 ▼
Open
 │
 ▼
Fixed
 │
 ▼
Retesting
 │
 ▼
Verified
 │
 ▼
Closed
```

If the defect still exists after Retesting:

```text
Retesting
     │
     ▼
Failed
     │
     ▼
Reopened
     │
     ▼
Assigned
```

---

## Defect Workflow

```text
Test Execution
       │
       ▼
Defect Identified
       │
       ▼
Create Defect Report
       │
       ▼
Assign to Developer
       │
       ▼
Developer Fixes Defect
       │
       ▼
Retesting
       │
  ┌────┴────┐
  │         │
Pass      Fail
  │         │
  ▼         ▼
Closed   Reopened
```

---

## Severity Levels

Severity indicates the **impact** of the defect on the application.

### Critical

The application crashes or major functionality is unavailable.

Example:

- Application crash
- Data loss

---

### Major

Important functionality is affected.

Example:

- Login failure
- Payment failure

---

### Minor

Small functionality is affected.

Example:

- Incorrect validation message

---

### Low

Cosmetic issues.

Example:

- Font alignment
- Color mismatch
- Typographical errors

---

## Priority Levels

Priority indicates **how quickly the defect should be fixed**.

### High

Must be fixed immediately.

---

### Medium

Should be fixed in the next release.

---

### Low

Can be fixed later.

---

## Severity vs Priority

| **Severity** | **Priority** |
|---------------|--------------|
| Measures the impact of the defect. | Measures the urgency of fixing the defect. |
| Decided mainly by the Test Engineer. | Usually decided by the Project Manager or Product Owner. |
| Related to software quality. | Related to business importance. |

---

## Common Defect Tracking Tools

| **Tool** | **Purpose** |
|-----------|-------------|
| JIRA | Issue Tracking and Project Management |
| Bugzilla | Open-source Bug Tracking |
| Mantis | Web-based Defect Tracking |

---

## Advantages of Defect Tracking

- **Maintains complete defect history.**
- **Improves communication between Testing and Development teams.**
- **Helps prioritize defect fixing.**
- **Supports Retesting and Regression Testing.**
- **Improves software quality.**
- **Provides project transparency.**

---

## Real-Time Example

Consider a **Gmail Login Application**.

Requirement:

The Password entered by the user should be masked using asterisks (*).

Actual Result:

The Password is displayed as plain text.

The Test Engineer reports the defect in **JIRA** with:

- Defect Summary
- Steps to Reproduce
- Screenshot
- Severity: Major
- Priority: High

The Developer fixes the issue, and the Test Engineer performs Retesting before closing the defect.

---

## Frequently Asked Interview Questions

### 1. What is Defect Tracking?

Defect Tracking is the process of identifying, recording, assigning, tracking, verifying, and managing software defects until they are closed.

---

### 2. Name some Defect Tracking tools.

- JIRA
- Bugzilla
- Mantis

---

### 3. What information is included in a Defect Report?

- Defect Number
- Defect Summary
- Steps to Reproduce
- Author
- Submission Date
- Version Number
- Build Number
- Assigned Developer
- Severity
- Screenshot

---

### 4. What is the difference between Severity and Priority?

**Severity** indicates the impact of the defect, whereas **Priority** indicates how urgently the defect should be fixed.

---

### 5. Which STLC phase follows Requirement Traceability Matrix?

**Defect Tracking.**

---

## Key Points

- **Defect Tracking records and manages software defects.**
- **Defects are reported through Email or Defect Tracking Tools.**
- **JIRA, Bugzilla, and Mantis are commonly used tools.**
- **Severity measures impact, while Priority measures urgency.**
- **Every reported defect passes through a defined lifecycle before closure.**

---

## Summary

**Defect Tracking** is the process of identifying, recording, assigning, tracking, and managing software defects throughout the Software Testing Life Cycle. Test Engineers report defects using emails or specialized tools such as **JIRA**, **Bugzilla**, and **Mantis**. Each defect contains detailed information, including its summary, reproduction steps, severity, priority, assigned developer, and supporting evidence. Effective Defect Tracking ensures timely defect resolution, improves communication between Testing and Development teams, and contributes to delivering high-quality software.
