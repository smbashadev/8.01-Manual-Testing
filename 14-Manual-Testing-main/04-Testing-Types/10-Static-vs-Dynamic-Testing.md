# Static Testing vs Dynamic Testing

## Introduction

Software Testing can be broadly classified into two categories: **Static Testing** and **Dynamic Testing**. Both techniques play an important role in identifying defects and improving software quality.

**Static Testing** focuses on evaluating software artifacts without executing the application, whereas **Dynamic Testing** involves executing the software to verify its behavior and functionality.

Understanding the differences between these two testing techniques helps Test Engineers choose the appropriate testing approach during different phases of the Software Development Life Cycle (SDLC).

---

## Static Testing

### Definition

**Static Testing** is the process of testing the software **without executing the application** or performing any action on it.

The primary objective of Static Testing is to identify defects in documents, requirements, design, source code, and other software artifacts before the application is executed.

### Examples

- **Graphical User Interface (GUI) Review**
- **Code Review**
- Requirement Review
- Design Review
- Walkthrough
- Inspection
- Document Review

---

## Characteristics of Static Testing

- **Does not require software execution.**
- **Performed during the early stages of development.**
- **Helps identify defects before coding and execution.**
- **Reduces the overall cost of fixing defects.**
- **Improves software quality at an early stage.**

---

## Advantages of Static Testing

- **Detects defects early in the SDLC.**
- **Reduces development cost.**
- **Improves software quality.**
- **Helps identify requirement and design issues.**
- **Prevents defects from reaching later testing phases.**

---

## Dynamic Testing

### Definition

**Dynamic Testing** is the process of testing the software **by executing the application and performing actions on it**.

The primary objective of Dynamic Testing is to verify whether the software behaves according to the specified requirements.

### Examples

- **Black Box Testing**
- **White Box Testing**
- **Grey Box Testing**
- Functional Testing
- Integration Testing
- System Testing
- Acceptance Testing

---

## Characteristics of Dynamic Testing

- **Requires execution of the application.**
- **Verifies actual software behavior.**
- **Checks inputs and outputs.**
- **Detects runtime defects.**
- **Validates software functionality.**

---

## Advantages of Dynamic Testing

- **Detects runtime errors.**
- **Verifies business requirements.**
- **Ensures software functionality.**
- **Identifies performance-related issues.**
- **Provides confidence before software release.**

---

## Comparison Table

| **Static Testing** | **Dynamic Testing** |
|--------------------|---------------------|
| Testing is performed **without executing** the software. | Testing is performed **by executing** the software. |
| Focuses on documents, design, and source code. | Focuses on software behavior and functionality. |
| Performed during the early stages of SDLC. | Performed after the software is developed. |
| Detects defects before execution. | Detects defects during software execution. |
| Does not require test data. | Requires test data for execution. |
| Faster and less expensive. | More time-consuming than Static Testing. |
| Prevents defects early. | Validates that the application works correctly. |
| Examples: Code Review, GUI Review, Walkthrough, Inspection. | Examples: Black Box Testing, White Box Testing, Functional Testing, System Testing. |

---

## Examples

### Static Testing Example

A Test Engineer reviews the **Software Requirement Specification (SRS)** document and identifies that the Login module requirements are incomplete.

No software is executed during this activity.

This is an example of **Static Testing**.

---

### Dynamic Testing Example

A Test Engineer launches a **Gmail Application**, enters a Username and Password, and clicks the **Login** button to verify whether the Inbox is displayed.

Since the application is executed, this is an example of **Dynamic Testing**.

---

## Real-Time Scenario

Suppose a company is developing an **Online Banking Application**.

### During Requirement Phase

The QA team reviews the requirement documents and identifies missing validation rules for the Login page.

This activity is **Static Testing**.

---

### During Testing Phase

After the application is developed, the QA team executes the Login functionality by entering valid and invalid credentials to verify the application's behavior.

This activity is **Dynamic Testing**.

---

## Frequently Asked Interview Questions

### 1. What is Static Testing?

Static Testing is the process of testing software without executing the application.

---

### 2. What is Dynamic Testing?

Dynamic Testing is the process of testing software by executing the application.

---

### 3. Give examples of Static Testing.

- Code Review
- GUI Review
- Requirement Review
- Walkthrough
- Inspection

---

### 4. Give examples of Dynamic Testing.

- Black Box Testing
- White Box Testing
- Grey Box Testing
- Functional Testing
- Integration Testing

---

### 5. Which testing technique detects defects earlier?

**Static Testing** detects defects earlier because it is performed before software execution.

---

## Key Points

- **Static Testing does not require software execution.**
- **Dynamic Testing requires software execution.**
- **Static Testing identifies defects in documents and code.**
- **Dynamic Testing validates software functionality.**
- **Both testing techniques improve software quality.**
- **Static and Dynamic Testing complement each other throughout the SDLC.**

---

## Summary

**Static Testing** and **Dynamic Testing** are two fundamental software testing techniques used throughout the Software Development Life Cycle. Static Testing focuses on reviewing software artifacts such as requirements, design documents, and source code without executing the application, helping detect defects early. Dynamic Testing verifies the application's behavior by executing the software and validating its functionality against the specified requirements. Together, these testing techniques improve software quality, reduce defects, and ensure reliable software delivery.
