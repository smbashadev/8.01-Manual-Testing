# Requirement Traceability Matrix (RTM)

## Introduction

A **Requirement Traceability Matrix (RTM)** is an important document in the Software Testing Life Cycle (STLC). It helps ensure that every customer requirement is covered by one or more Test Cases and that every reported defect can be traced back to the corresponding Test Case.

The Traceability Matrix improves requirement coverage, simplifies defect tracking, and helps verify that no requirement is left untested.

---

## Definition

A **Traceability Matrix** is a document that maps between the **Requirement Number** and the **Test Case ID**, or sometimes between the **Defect Number** and the **Test Case ID**.

Depending on the area of mapping, the Traceability Matrix is divided into two types:

1. **Requirement Traceability Matrix (RTM)**
2. **Defect Traceability Matrix (DTM)**

---

## Objectives of Traceability Matrix

The Traceability Matrix is prepared to:

- **Ensure complete requirement coverage.**
- **Verify that every requirement has corresponding Test Cases.**
- **Track defects efficiently.**
- **Support Retesting and Regression Testing.**
- **Improve testing quality and project visibility.**

---

# Types of Traceability Matrix

## 1. Requirement Traceability Matrix (RTM)

### Definition

A **Requirement Traceability Matrix (RTM)** is a document that maps between the **Requirement Number** and the **Test Case ID**.

It is prepared to verify whether **every requirement has at least one associated Test Case**.

This ensures that no customer requirement is missed during testing.

---

## Sample Requirement Traceability Matrix

| **Requirement Number** | **Test Case ID** |
|------------------------|------------------|
| 1, 2, 3 | FT-01 |
| 4, 5, 6, 7 | FT-02 |
| 8 – 20 | IT-03 |
| 21 – 35 | ST-04 |
| 36 – 45 | LT-05 |
| 46 – 50 | ST-06 |

---

## Requirement Traceability Workflow

```text
Customer Requirements
          │
          ▼
Prepare Test Cases
          │
          ▼
Map Requirement Number
with Test Case ID
          │
          ▼
Verify Requirement Coverage
          │
          ▼
All Requirements Covered
```

---

## Benefits of RTM

- **Ensures complete requirement coverage.**
- **Identifies missing Test Cases.**
- **Improves requirement verification.**
- **Supports project audits.**
- **Helps estimate testing progress.**

---

# 2. Defect Traceability Matrix (DTM)

## Definition

A **Defect Traceability Matrix (DTM)** is a document that maps between the **Defect Number** and the **Test Case ID**.

It is mainly used to identify which Test Case reported a defect and to re-execute those Test Cases after the defect has been fixed.

---

## Sample Defect Traceability Matrix

| **Defect Number** | **Test Case ID** |
|-------------------|------------------|
| 01 (L) | FT-02 |
| 02 (H) | FT-05 |
| 03 (H) | IT-01 |
| 04 (L) | IT-06 |
| 05 (H) | PT-05 |
| 06 (L) | ST-05 |
| 07 (L) | ST-07 |

**Legend**

- **H** – High Severity
- **L** – Low Severity

---

## Defect Traceability Workflow

```text
Execute Test Cases
        │
        ▼
Defect Found
        │
        ▼
Assign Defect Number
        │
        ▼
Map Defect Number
with Test Case ID
        │
        ▼
Developer Fixes Defect
        │
        ▼
Retest Associated Test Case
```

---

## Importance of Defect Traceability Matrix

The Defect Traceability Matrix helps:

- **Track reported defects.**
- **Identify affected Test Cases.**
- **Support Retesting activities.**
- **Verify defect fixes.**
- **Maintain defect history.**

---

## Difference Between RTM and DTM

| **Requirement Traceability Matrix (RTM)** | **Defect Traceability Matrix (DTM)** |
|-------------------------------------------|--------------------------------------|
| Maps Requirement Number with Test Case ID. | Maps Defect Number with Test Case ID. |
| Ensures every requirement is tested. | Ensures every defect is tracked. |
| Used during Test Case preparation. | Used after defect reporting. |
| Helps identify missing Test Cases. | Helps identify affected Test Cases. |
| Supports requirement coverage. | Supports Retesting and defect verification. |

---

## Advantages of Traceability Matrix

- **Ensures 100% requirement coverage.**
- **Improves testing quality.**
- **Supports defect tracking.**
- **Makes Retesting easier.**
- **Improves project visibility.**
- **Helps during project audits.**
- **Reduces the possibility of missing requirements.**

---

## Real-Time Example

Consider an **Online Banking Application**.

Requirement:

```text
REQ-101

User should be able to transfer money.
```

Associated Test Cases:

```text
FT-021
FT-022
FT-023
```

Suppose **FT-022** fails during execution.

A defect is logged as:

```text
BUG-145
```

The Traceability Matrix stores:

```text
Requirement

REQ-101 → FT-021, FT-022, FT-023
```

```text
Defect

BUG-145 → FT-022
```

After the Developer fixes **BUG-145**, only the related Test Cases are re-executed.

---

## Frequently Asked Interview Questions

### 1. What is a Traceability Matrix?

A Traceability Matrix is a document used to establish relationships between Requirements, Test Cases, and Defects.

---

### 2. What are the two types of Traceability Matrix?

- Requirement Traceability Matrix (RTM)
- Defect Traceability Matrix (DTM)

---

### 3. Why is RTM prepared?

RTM is prepared to ensure that every requirement has at least one corresponding Test Case.

---

### 4. Why is DTM prepared?

DTM is prepared to track reported defects and identify the associated Test Cases for Retesting.

---

### 5. Which STLC phase follows Test Execution?

**Requirement Traceability Matrix (RTM).**

---

## Key Points

- **RTM maps Requirements with Test Cases.**
- **DTM maps Defects with Test Cases.**
- **RTM ensures complete requirement coverage.**
- **DTM supports Retesting after defect fixes.**
- **Traceability Matrix improves software quality and testing efficiency.**

---

## Summary

A **Traceability Matrix** is an important document in the Software Testing Life Cycle that establishes relationships between Requirements, Test Cases, and Defects. It consists of the **Requirement Traceability Matrix (RTM)**, which ensures every requirement is covered by one or more Test Cases, and the **Defect Traceability Matrix (DTM)**, which maps defects to their corresponding Test Cases for efficient Retesting and defect verification. Maintaining a Traceability Matrix helps improve requirement coverage, defect tracking, project transparency, and overall software quality.
