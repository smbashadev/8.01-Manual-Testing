# Functional Testing vs Non-Functional Testing

## Introduction

Software Testing is broadly classified into two major categories:

- **Functional Testing**
- **Non-Functional Testing**

Functional Testing verifies whether the software performs the expected business functionalities according to the specified requirements. Non-Functional Testing verifies the quality attributes of the software, such as performance, security, usability, and compatibility.

Both testing techniques are equally important for delivering a high-quality software product.

---

# Functional Testing

## Definition

**Functional Testing** is a type of software testing in which the Test Engineer verifies whether the **business functionalities** of the software application work according to the specified requirements.

It focuses on validating **what the software does**.

---

## Objectives of Functional Testing

Functional Testing is performed to:

- **Verify business requirements.**
- **Validate application functionality.**
- **Ensure correct input and output.**
- **Identify functional defects.**
- **Confirm software behaves as expected.**

---

## Types of Functional Testing

Functional Testing includes:

- Black Box Testing
- White Box Testing
- Smoke Testing
- Sanity Testing
- Regression Testing
- Retesting
- Integration Testing
- System Testing
- Acceptance Testing

---

## Examples of Functional Testing

- Login functionality
- Registration functionality
- Payment processing
- Search functionality
- Email sending
- Password reset
- Fund transfer in Banking Applications

---

# Non-Functional Testing

## Definition

**Non-Functional Testing** is a type of software testing in which the Test Engineer verifies the **quality attributes** of a software application.

It focuses on evaluating **how well the software performs** rather than what it does.

---

## Objectives of Non-Functional Testing

Non-Functional Testing is performed to:

- **Measure application performance.**
- **Verify software security.**
- **Evaluate usability.**
- **Check compatibility across environments.**
- **Assess reliability and recovery.**
- **Improve user experience.**

---

## Types of Non-Functional Testing

Non-Functional Testing includes:

- Performance Testing
- Security Testing
- Usability Testing
- Compatibility Testing
- Recovery Testing
- Globalization Testing
- Localization Testing
- Internationalization Testing

---

## Examples of Non-Functional Testing

- Measuring website response time.
- Verifying application security.
- Checking browser compatibility.
- Testing application recovery after a crash.
- Verifying multilingual support.
- Measuring application performance under heavy load.

---

# Comparison Table

| **Functional Testing** | **Non-Functional Testing** |
|-------------------------|----------------------------|
| Tests the **business functionality** of the software or application. | Tests the **quality attributes** of the software or application. |
| Verifies **what the software does**. | Verifies **how well the software performs**. |
| Based on functional requirements. | Based on non-functional requirements. |
| Checks inputs, outputs, and business logic. | Checks performance, security, usability, reliability, and compatibility. |
| Ensures application behaves according to customer requirements. | Ensures the application meets quality standards. |
| Performed before software release. | Usually performed after functional testing. |
| Example: Login, Registration, Payment, Search. | Example: Performance, Security, Compatibility, Recovery. |
| Helps validate application functionality. | Helps improve overall software quality. |

---

## Functional Testing Workflow

```text
Requirement
      │
      ▼
Prepare Test Cases
      │
      ▼
Execute Functional Tests
      │
      ▼
Expected Output?
   ┌───┴───┐
   │       │
 Yes       No
  │         │
  ▼         ▼
Pass     Report Defect
```

---

## Non-Functional Testing Workflow

```text
Application Ready
        │
        ▼
Measure Quality Attributes
        │
        ▼
Performance
Security
Usability
Compatibility
Recovery
        │
        ▼
Evaluate Results
        │
        ▼
Application Quality Verified
```

---

## Real-Time Example

Consider an **Online Banking Application**.

### Functional Testing

The Test Engineer verifies:

- Login
- Fund Transfer
- Balance Enquiry
- Mini Statement
- Logout

The objective is to ensure that each business functionality works correctly.

---

### Non-Functional Testing

The Test Engineer verifies:

- Login response time.
- Security of customer accounts.
- Browser compatibility.
- Application recovery after server failure.
- User friendliness of the interface.

The objective is to evaluate the quality of the application.

---

## Advantages of Functional Testing

- **Ensures business requirements are satisfied.**
- **Identifies functional defects.**
- **Improves software correctness.**
- **Validates customer requirements.**
- **Increases software reliability.**

---

## Advantages of Non-Functional Testing

- **Improves software performance.**
- **Enhances application security.**
- **Improves user experience.**
- **Ensures compatibility across environments.**
- **Increases software stability and reliability.**

---

## Frequently Asked Interview Questions

### 1. What is Functional Testing?

Functional Testing verifies whether the business functionalities of a software application work according to the specified requirements.

---

### 2. What is Non-Functional Testing?

Non-Functional Testing verifies the quality attributes of a software application, such as performance, security, usability, compatibility, and reliability.

---

### 3. Give examples of Functional Testing.

- Black Box Testing
- White Box Testing
- Smoke Testing
- Sanity Testing
- Regression Testing
- Retesting

---

### 4. Give examples of Non-Functional Testing.

- Performance Testing
- Security Testing
- Compatibility Testing
- Usability Testing
- Recovery Testing
- Globalization Testing

---

### 5. What is the main difference between Functional and Non-Functional Testing?

**Functional Testing verifies what the application does, whereas Non-Functional Testing verifies how well the application performs.**

---

## Key Points

- **Functional Testing verifies business functionality.**
- **Non-Functional Testing verifies software quality attributes.**
- **Functional Testing checks application behavior.**
- **Non-Functional Testing checks performance, security, usability, and compatibility.**
- **Both testing techniques are essential for delivering high-quality software.**

---

## Summary

**Functional Testing** and **Non-Functional Testing** are the two primary categories of software testing. Functional Testing ensures that the software performs all required business functionalities according to the specified requirements, while Non-Functional Testing evaluates important quality attributes such as performance, security, usability, compatibility, and reliability. Together, these testing approaches help deliver software that is both functionally correct and capable of providing a secure, efficient, and user-friendly experience.
