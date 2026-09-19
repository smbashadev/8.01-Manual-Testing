# Testing Types Overview

## Introduction

Software Testing consists of various testing techniques that help verify the quality, reliability, functionality, and performance of a software application.

Different testing types are used based on the purpose of testing. Each testing type focuses on a specific aspect of the software to ensure that it satisfies customer requirements and delivers a high-quality product.

Understanding the different testing types is essential for every Software Test Engineer because each testing technique plays an important role during the Software Testing Life Cycle (STLC).

---

## Definition

**Testing Types** are different software testing techniques used to verify and validate the quality, functionality, performance, security, usability, and reliability of a software application.

Each testing type has a specific objective and is performed during different stages of software development and testing.

---

## Classification of Testing

Software Testing is broadly classified into the following categories:

1. **Black Box Testing**
2. **White Box Testing**
3. **Grey Box Testing**

---

## Overview Diagram

```text
                     Types of Testing
                            │
        ┌───────────────────┼───────────────────┐
        │                   │                   │
        ▼                   ▼                   ▼
 Black Box Testing    White Box Testing    Grey Box Testing
```

---

## 1. Black Box Testing

### Definition

**Black Box Testing** is a software testing technique in which the tester verifies the application's functionality without having knowledge of the internal source code, program structure, or implementation details.

The tester focuses only on:

- Inputs
- Outputs
- Functional Requirements
- Expected Results

This testing is mainly performed by **Software Test Engineers (QA Engineers)**.

---

## 2. White Box Testing

### Definition

**White Box Testing** is a software testing technique in which the tester has complete knowledge of the application's internal code, program logic, algorithms, and implementation.

The tester verifies:

- Source Code
- Statements
- Conditions
- Loops
- Execution Paths

This testing is generally performed by **Developers**.

---

## 3. Grey Box Testing

### Definition

**Grey Box Testing** is a software testing technique that combines the concepts of both Black Box Testing and White Box Testing.

The tester has partial knowledge of the application's internal implementation while also verifying its external functionality.

Grey Box Testing helps identify defects that may not be detected by using only Black Box or White Box Testing.

---

## Comparison of Testing Types

| **Testing Type** | **Knowledge of Source Code** | **Performed By** | **Primary Focus** |
|------------------|------------------------------|------------------|-------------------|
| **Black Box Testing** | No | Test Engineers | Functionality |
| **White Box Testing** | Yes | Developers | Source Code and Program Logic |
| **Grey Box Testing** | Partial | Developers / Test Engineers | Both Functionality and Internal Logic |

---

## Real-Time Example

Consider an **Online Banking Application**.

### Black Box Testing

The tester verifies:

- Login
- Fund Transfer
- Balance Enquiry
- Transaction History

without viewing the source code.

### White Box Testing

The developer verifies:

- Program Logic
- Conditions
- Loops
- Exception Handling

by reviewing and testing the source code.

### Grey Box Testing

The tester has limited knowledge of the database and application architecture while testing features such as fund transfers and transaction processing.

---

## Key Points

- **Software Testing is classified into Black Box Testing, White Box Testing, and Grey Box Testing.**
- **Black Box Testing focuses on application functionality.**
- **White Box Testing focuses on source code and program logic.**
- **Grey Box Testing combines Black Box and White Box Testing techniques.**
- **Each testing type serves a different purpose during software testing.**

---

## Summary

Software Testing includes different testing techniques that help ensure software quality from multiple perspectives. **Black Box Testing** validates application functionality, **White Box Testing** verifies the internal code and logic, and **Grey Box Testing** combines both approaches to provide more comprehensive testing. Understanding these testing types forms the foundation for learning advanced software testing techniques.
