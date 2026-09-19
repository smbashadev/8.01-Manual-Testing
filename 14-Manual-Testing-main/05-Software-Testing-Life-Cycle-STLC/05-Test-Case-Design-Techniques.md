# Test Case Design Techniques

## Introduction

Writing effective Test Cases is one of the most important responsibilities of a Software Test Engineer. A good Test Case should identify maximum defects while minimizing the total number of Test Cases.

To achieve this objective, Test Engineers use **Test Case Design Techniques**. These techniques help create efficient, optimized, and systematic Test Cases that provide maximum test coverage.

---

## Definition

**Test Case Design Techniques** are systematic methods used to write effective Test Cases for verifying the functionality of a software application.

These techniques help Test Engineers reduce duplicate Test Cases, improve test coverage, and identify defects efficiently.

---

## Objectives of Test Case Design Techniques

Test Case Design Techniques are used to:

- **Reduce the total number of Test Cases.**
- **Improve requirement coverage.**
- **Identify maximum defects with minimum effort.**
- **Avoid redundant Test Cases.**
- **Improve testing efficiency.**
- **Provide systematic testing.**

---

## Types of Test Case Design Techniques

There are three major Test Case Design Techniques.

1. **Boundary Value Analysis (BVA)**
2. **Equivalence Class Partitioning (ECP)**
3. **Error Guessing**

---

# 1. Boundary Value Analysis (BVA)

## Definition

**Boundary Value Analysis (BVA)** is a Test Case Design Technique in which Test Cases are prepared using the **boundary values** of the input range.

In this technique, Test Engineers first consider:

- Minimum Boundary Value
- Maximum Boundary Value
- Nominal (Valid) Values
- One value below the minimum
- One value above the maximum

Most software defects occur at boundary conditions; therefore, Boundary Value Analysis is highly effective.

---

## Functional Requirements

### Gmail Login Module

1. **Username** should contain a minimum of **3 characters** and a maximum of **7 characters**.

2. **Password** should contain a minimum of **3 characters** and a maximum of **7 characters**.

3. **Special characters are not allowed in the Password.**

4. After clicking **Login**, the **Inbox** should be displayed.

---

## Boundary Value Analysis Example

| **Input Length** | **Value Type** | **Expected Result** |
|-----------------:|----------------|---------------------|
| 2 Characters | One Less Than Minimum | Invalid |
| 3 Characters | Minimum Boundary | Valid |
| 4 Characters | Nominal Value | Valid |
| 5 Characters | Nominal Value | Valid |
| 6 Characters | Nominal Value | Valid |
| 7 Characters | Maximum Boundary | Valid |
| 8 Characters | One More Than Maximum | Invalid |

---

## Sample Test Cases

| **Test Case ID** | **Username Length** | **Expected Result** |
|------------------|--------------------:|---------------------|
| BVA-01 | 2 | Invalid Username |
| BVA-02 | 3 | Valid |
| BVA-03 | 5 | Valid |
| BVA-04 | 7 | Valid |
| BVA-05 | 8 | Invalid Username |

---

## Advantages of Boundary Value Analysis

- **Detects boundary-related defects.**
- **Reduces the number of Test Cases.**
- **Provides good test coverage.**
- **Simple to understand and implement.**

---

# 2. Equivalence Class Partitioning (ECP)

## Definition

**Equivalence Class Partitioning (ECP)** is a Test Case Design Technique in which the input data is divided into different **equivalence classes (partitions)**.

Instead of testing every possible input, one representative value is selected from each class.

This technique reduces the total number of Test Cases while maintaining effective coverage.

---

## Classification of Input Data

The input values are divided into three categories.

```text
                Input Values

        ┌─────────┬─────────┬─────────┐
        │         │         │
        ▼         ▼         ▼

 Under Value  Nominal Value  Over Value
 (Invalid)      (Valid)      (Invalid)
```

---

## Example

Suppose the Username length should be **3 to 7 characters**.

### Class 1 – Under Value

Invalid values less than the minimum.

| Input | Status |
|-------:|--------|
| 1 Character | Invalid |
| 2 Characters | Invalid |

---

### Class 2 – Nominal Value

Valid values within the specified range.

| Input | Status |
|-------:|--------|
| 3 Characters | Valid |
| 4 Characters | Valid |
| 5 Characters | Valid |
| 6 Characters | Valid |
| 7 Characters | Valid |

---

### Class 3 – Over Value

Invalid values greater than the maximum.

| Input | Status |
|-------:|--------|
| 8 Characters | Invalid |
| 9 Characters | Invalid |

---

## Advantages of Equivalence Class Partitioning

- **Reduces unnecessary Test Cases.**
- **Improves testing efficiency.**
- **Provides good requirement coverage.**
- **Easy to design Test Cases.**

---

# 3. Error Guessing

## Definition

**Error Guessing** is a Test Case Design Technique based on the **experience**, **expertise**, and **knowledge** of the Test Engineer.

The Test Engineer predicts areas where defects are likely to occur and prepares Test Cases accordingly.

Unlike other techniques, Error Guessing does not follow predefined rules.

Its success depends entirely on the tester's experience.

---

## Characteristics

- Experience-based testing.
- No predefined rules.
- Helps identify hidden defects.
- Complements other Test Case Design Techniques.

---

## Examples

An experienced Test Engineer may verify the following scenarios.

- Leaving mandatory fields blank.
- Entering only spaces.
- Entering special characters.
- Entering SQL Injection statements.
- Copy-paste operations.
- Extremely large input values.
- Browser refresh after form submission.
- Double-clicking the Login button.
- Network interruption during submission.

---

## Test Case Review Example

After preparing Test Cases, another Test Engineer reviews them.

### Review Document

| **Test Case ID** | **Comment** |
|------------------|-------------|
| FT-01 | The Test Case is in accordance with the requirement. |

---

## Comparison of Test Case Design Techniques

| **Boundary Value Analysis** | **Equivalence Class Partitioning** | **Error Guessing** |
|-----------------------------|------------------------------------|--------------------|
| Focuses on boundary values. | Focuses on input partitions. | Focuses on tester experience. |
| Uses minimum and maximum values. | Uses representative values from each class. | Uses intuition and expertise. |
| Rule-based technique. | Rule-based technique. | Experience-based technique. |
| Detects boundary defects. | Reduces Test Cases. | Detects hidden defects. |

---

## Test Case Design Workflow

```text
Requirement Study
        │
        ▼
Select Test Case Design Technique
        │
        ▼
Boundary Value Analysis
Equivalence Class Partitioning
Error Guessing
        │
        ▼
Prepare Test Cases
        │
        ▼
Review Test Cases
        │
        ▼
Approval
```

---

## Advantages of Test Case Design Techniques

- **Reduce the number of Test Cases.**
- **Increase testing efficiency.**
- **Improve requirement coverage.**
- **Help identify defects systematically.**
- **Save testing time and effort.**

---

## Real-Time Example

Consider an **Online Banking Application**.

Requirement:

"The ATM PIN should contain exactly 4 digits."

The Test Engineer applies:

- **Boundary Value Analysis** to verify values around the allowed length.
- **Equivalence Class Partitioning** to divide valid and invalid PIN lengths.
- **Error Guessing** to test alphabetic characters, special symbols, blank values, and copied PINs.

Together, these techniques provide comprehensive test coverage.

---

## Frequently Asked Interview Questions

### 1. What are Test Case Design Techniques?

They are systematic methods used to prepare effective and optimized Test Cases.

---

### 2. Name the three Test Case Design Techniques.

- Boundary Value Analysis (BVA)
- Equivalence Class Partitioning (ECP)
- Error Guessing

---

### 3. Which technique uses minimum and maximum values?

**Boundary Value Analysis (BVA).**

---

### 4. Which technique divides input data into valid and invalid classes?

**Equivalence Class Partitioning (ECP).**

---

### 5. Which technique depends on the Test Engineer's experience?

**Error Guessing.**

---

## Key Points

- **Test Case Design Techniques improve testing efficiency.**
- **Boundary Value Analysis focuses on boundary conditions.**
- **Equivalence Class Partitioning divides inputs into logical groups.**
- **Error Guessing depends on tester experience and expertise.**
- **Using these techniques reduces redundant Test Cases and improves software quality.**

---

## Summary

**Test Case Design Techniques** are systematic approaches used by Test Engineers to create effective and optimized Test Cases. The three major techniques are **Boundary Value Analysis (BVA)**, which focuses on boundary values, **Equivalence Class Partitioning (ECP)**, which divides input data into valid and invalid classes, and **Error Guessing**, which relies on the experience and expertise of the Test Engineer to identify likely defect areas. Together, these techniques improve testing efficiency, reduce unnecessary Test Cases, and enhance software quality.
