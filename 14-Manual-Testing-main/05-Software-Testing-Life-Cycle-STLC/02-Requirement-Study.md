# Requirement Study

## Introduction

The first phase of the **Software Testing Life Cycle (STLC)** is **Requirement Study**. Before writing test cases or executing tests, the Testing Team must thoroughly understand the software requirements.

A clear understanding of the requirements helps Test Engineers identify testable scenarios, prepare effective test cases, estimate testing effort, and ensure that customer expectations are fulfilled.

Requirement Study is one of the most important phases because incorrect understanding of requirements may lead to incomplete testing and software defects.

---

## Definition

**Requirement Study** is the process in which a Test Engineer studies and understands the project requirements in order to perform software testing effectively.

The requirements provided to the Test Engineer serve as the foundation for designing Test Cases and planning the testing activities.

---

## Objectives of Requirement Study

Requirement Study is performed to:

- **Understand the business requirements.**
- **Identify testable functionalities.**
- **Clarify ambiguous requirements.**
- **Understand the scope of testing.**
- **Prepare accurate Test Cases.**
- **Reduce defects caused by misunderstanding requirements.**

---

## Requirement Documents

The requirements are provided to the Test Engineer in one or more of the following formats.

### I. Customer Requirement Specification (CRS)

**Customer Requirement Specification (CRS)** contains the requirements collected directly from the customer.

It describes:

- Customer expectations
- Business needs
- High-level requirements
- Project objectives

CRS is generally prepared during the initial stage of the project.

---

### II. Software Requirement Specification (SRS)

**Software Requirement Specification (SRS)** is a detailed document prepared after analyzing the customer requirements.

It contains:

- Functional Requirements
- Non-Functional Requirements
- System Features
- Constraints
- Business Rules
- Acceptance Criteria

The SRS document acts as the primary reference for both Developers and Test Engineers.

---

### III. Functional Requirement Specification (FRS)

**Functional Requirement Specification (FRS)** describes the functional behavior of every module in the application.

It explains:

- Inputs
- Processing
- Outputs
- Functional Logic
- Validation Rules

The Test Engineer mainly refers to the FRS while preparing Test Cases.

---

### IV. Use Case Diagram

A **Use Case Diagram** is a UML (Unified Modeling Language) diagram that represents the interaction between **Actors** and the **Functionalities** of a software application.

It specifies **which actor performs which functionality** within the application.

---

## Use Case Diagram

### ATM System Example

```text
                     +--------------------------------------+
                     |             ATM System               |
                     |                                      |
Customer ----------->| (Check Balance)                     |
Customer ----------->| (Withdraw Cash)                     |
Customer ----------->| (Deposit Money)                     |
Customer ----------->| (Mini Statement)                    |
Customer ----------->| (Change PIN)                        |
                     |                                      |
Bank Technician ---->| (Maintenance)                       |
Bank Technician ---->| (Repair)                            |
                     +--------------------------------------+
```

### Actors

- **Customer**
- **Bank Technician**

### Functionalities

- Check Balance
- Withdraw Cash
- Deposit Money
- Mini Statement
- Change PIN
- Maintenance
- Repair

---

## Activities Performed During Requirement Study

During this phase, the Test Engineer performs the following activities:

- Study requirement documents.
- Understand business functionality.
- Identify functional and non-functional requirements.
- Clarify unclear requirements with the Business Analyst or Product Owner.
- Identify testable scenarios.
- Estimate testing effort.
- Prepare for Test Planning.

---

## Deliverables

The Requirement Study phase produces:

- Requirement Analysis Notes
- Requirement Clarifications
- List of Testable Requirements
- Requirement Understanding Document
- Inputs for Test Planning

---

## Importance of Requirement Study

Requirement Study is important because it:

- **Provides a clear understanding of the project.**
- **Helps prepare accurate Test Cases.**
- **Prevents requirement misunderstandings.**
- **Reduces testing defects.**
- **Improves software quality.**
- **Ensures complete requirement coverage.**

---

## Real-Time Example

Consider an **Online Banking Application**.

The customer specifies the following requirements:

- Users should be able to log in.
- Users should transfer money securely.
- Users should check account balance.
- Users should download account statements.

The Test Engineer studies these requirements through the **CRS**, **SRS**, **FRS**, and **Use Case Diagram** before preparing Test Cases.

---

## Frequently Asked Interview Questions

### 1. What is Requirement Study?

Requirement Study is the process of understanding software requirements before starting software testing.

---

### 2. What are the different requirement documents used in STLC?

- Customer Requirement Specification (CRS)
- Software Requirement Specification (SRS)
- Functional Requirement Specification (FRS)
- Use Case Diagram

---

### 3. What is CRS?

CRS (Customer Requirement Specification) contains the customer's business requirements and expectations.

---

### 4. What is SRS?

SRS (Software Requirement Specification) is a detailed document describing the software requirements for development and testing.

---

### 5. What is FRS?

FRS (Functional Requirement Specification) describes the functional behavior of each module in the application.

---

### 6. What is a Use Case Diagram?

A Use Case Diagram is a UML diagram that represents the interaction between actors and the functionalities of a software application.

---

### 7. Why is Requirement Study important?

Because it helps Test Engineers understand the application completely before designing Test Cases and performing testing.

---

## Key Points

- **Requirement Study is the first phase of STLC.**
- **It helps Test Engineers understand software requirements.**
- **Requirements may be provided as CRS, SRS, FRS, or Use Case Diagrams.**
- **Use Case Diagrams show the interaction between actors and system functionalities.**
- **A good Requirement Study reduces testing errors and improves software quality.**

---

## Summary

**Requirement Study** is the first phase of the Software Testing Life Cycle in which Test Engineers analyze and understand the software requirements before starting testing activities. The requirements are commonly provided through **Customer Requirement Specification (CRS)**, **Software Requirement Specification (SRS)**, **Functional Requirement Specification (FRS)**, and **Use Case Diagrams**. A proper understanding of these documents enables the Testing Team to prepare effective Test Cases, ensure complete requirement coverage, and deliver high-quality software.
