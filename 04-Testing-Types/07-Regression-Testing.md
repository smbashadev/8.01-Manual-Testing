# Regression Testing

## Introduction

Software applications are continuously enhanced by adding new features, fixing bugs, and improving existing functionality. Every change made to the application may unintentionally affect previously working features.

To ensure that existing functionalities continue to work correctly after every modification, **Regression Testing** is performed.

Regression Testing helps verify that newly introduced changes have not negatively impacted the existing functionality of the software.

---

## Definition

**Regression Testing** is the process of testing the software repeatedly by **re-executing previously executed test cases on different software builds** to ensure that existing functionalities continue to work correctly after changes, bug fixes, or enhancements.

Regression Testing is usually performed whenever:

- A new build is received.
- A bug is fixed.
- A new feature is added.
- Existing functionality is modified.
- Software maintenance is performed.

---

## Objectives of Regression Testing

Regression Testing is performed to:

- **Verify that existing functionalities remain unaffected.**
- **Ensure bug fixes do not introduce new defects.**
- **Maintain software stability.**
- **Validate software quality after every build.**
- **Increase customer confidence.**

---

## Types of Regression Testing

Based on the area of testing, Regression Testing is classified into three types:

1. **Full Regression Testing**
2. **Unit Regression Testing**
3. **Regional Regression Testing**

---

# 1. Full Regression Testing

## Definition

**Full Regression Testing** is the process of executing **all existing test cases** along with the test cases for newly added modules.

It is generally performed when major changes are made to the application or when multiple modules are affected.

---

## Example

### Build 1

| Module | Test Cases |
|---------|-----------:|
| Login | 20 |
| Inbox | 20 |
| Compose | 20 |
| Draft | 10 |
| Sent Message | 10 |
| Trash | 10 |
| **Total** | **90 Test Cases** |

---

### Build 2

A new module called **Bin** is added.

| Module | Test Cases |
|---------|-----------:|
| Login | 20 |
| Inbox | 20 |
| Compose | 20 |
| Draft | 10 |
| Sent Message | 10 |
| Trash | 10 |
| Bin | 10 |
| **Total** | **100 Test Cases** |

All 100 test cases are executed.

This is called **Full Regression Testing**.

---

## When to Perform

Perform Full Regression Testing when:

- Major functionality changes occur.
- New modules are added.
- Multiple modules are modified.
- Before software release.

---

# 2. Unit Regression Testing

## Definition

**Unit Regression Testing** is the process of performing Regression Testing **only on the affected module** or on a **single unit**.

Instead of executing all test cases, only the modified module is tested.

---

## Example

### Build 1

| Module | Test Cases |
|---------|-----------:|
| Login | 20 |
| Inbox | 20 |
| Compose | 20 |
| Draft | 10 |
| Sent Message | 10 |
| Trash | 10 |
| **Total** | **90 Test Cases** |

---

### Build 2

Only the **Compose** module is modified.

| Module | Test Cases Executed |
|---------|--------------------:|
| Compose | 20 |
| **Total** | **20 Test Cases** |

Only the affected module is tested.

This is called **Unit Regression Testing**.

---

## When to Perform

Perform Unit Regression Testing when:

- A minor defect is fixed.
- Only one module is modified.
- The change has no impact on other modules.

---

# 3. Regional Regression Testing

## Definition

**Regional Regression Testing** is the process of performing Regression Testing on the **affected module** along with its **related modules** when the defect is considered major.

Instead of testing the complete application, only the impacted functional area is tested.

---

## Example

### Build 1

| Module | Test Cases |
|---------|-----------:|
| Login | 30 |
| Inbox | 10 |
| Compose | 20 |
| Draft | 10 |
| Sent Message | 10 |
| Trash | 10 |
| Bin | 10 |
| **Total** | **100 Test Cases** |

---

### Build 2

Suppose the **Compose** module is modified.

Since **Draft** and **Sent Message** are directly related to Compose, all three modules are tested.

| Module | Test Cases Executed |
|---------|--------------------:|
| Compose | 20 |
| Draft | 10 |
| Sent Message | 10 |
| **Total** | **40 Test Cases** |

This is called **Regional Regression Testing**.

---

## When to Perform

Perform Regional Regression Testing when:

- A major defect is fixed.
- Related modules may also be affected.
- The impact of the change extends beyond a single module.

---

## Comparison of Regression Testing Types

| **Full Regression Testing** | **Unit Regression Testing** | **Regional Regression Testing** |
|-----------------------------|-----------------------------|---------------------------------|
| Tests all modules. | Tests only one affected module. | Tests the affected module and related modules. |
| Time-consuming. | Fastest approach. | Moderate testing effort. |
| Provides maximum confidence. | Suitable for minor changes. | Suitable for major defects affecting related modules. |
| Executes all test cases. | Executes only unit-specific test cases. | Executes affected and dependent module test cases. |

---

## Advantages of Regression Testing

- **Ensures existing functionality remains stable.**
- **Detects side effects caused by code changes.**
- **Improves software reliability.**
- **Reduces production defects.**
- **Supports continuous software development.**
- **Increases customer confidence.**
- **Maintains software quality after every build.**

---

## Disadvantages of Regression Testing

- **Time-consuming for large applications.**
- **Requires repeated execution of test cases.**
- **May increase testing effort.**
- **Can be costly if performed manually.**

---

## Practical Example

Consider an **Online Shopping Application**.

The application contains the following modules:

- Login
- Product Search
- Shopping Cart
- Payment
- Order History

### Scenario 1

A new **Wishlist Module** is added.

The QA team executes all existing test cases along with the Wishlist test cases.

This is **Full Regression Testing**.

---

### Scenario 2

Only the **Payment Module** is modified.

The QA team tests only the Payment module.

This is **Unit Regression Testing**.

---

### Scenario 3

The **Shopping Cart Module** is modified.

Since Shopping Cart directly interacts with **Payment** and **Order History**, all three modules are tested.

This is **Regional Regression Testing**.

---

## Frequently Asked Interview Questions

### 1. What is Regression Testing?

Regression Testing is the process of re-executing previously executed test cases on different software builds to ensure existing functionality continues to work correctly.

---

### 2. Why is Regression Testing performed?

To ensure that software modifications do not introduce new defects into existing functionality.

---

### 3. Name the three types of Regression Testing.

- Full Regression Testing
- Unit Regression Testing
- Regional Regression Testing

---

### 4. Which Regression Testing type requires the maximum effort?

**Full Regression Testing.**

---

### 5. Which Regression Testing type is performed for a minor bug fix?

**Unit Regression Testing.**

---

### 6. Which Regression Testing type is performed for a major defect affecting related modules?

**Regional Regression Testing.**

---

## Key Points

- **Regression Testing verifies existing functionality after software changes.**
- **Previously executed test cases are re-executed.**
- **Three types: Full, Unit, and Regional Regression Testing.**
- **Full Regression Testing covers the complete application.**
- **Unit Regression Testing focuses on a single affected module.**
- **Regional Regression Testing verifies affected and related modules.**
- **Regression Testing helps maintain software quality throughout development.**

---

## Summary

**Regression Testing** is an essential software testing technique used to ensure that existing functionality continues to work correctly after bug fixes, feature additions, or application enhancements. By re-executing previously executed test cases across different software builds, Regression Testing helps detect unintended side effects and maintain software stability. Depending on the scope of the changes, Regression Testing can be performed as **Full Regression Testing**, **Unit Regression Testing**, or **Regional Regression Testing**, each serving a specific purpose in maintaining software quality.
