# Adhoc Testing

## Introduction

Not all software defects can be identified using predefined Test Cases. Sometimes, Test Engineers intentionally perform random and unexpected actions on the application to evaluate its stability and discover hidden defects.

**Adhoc Testing** is an informal testing technique in which the Test Engineer performs testing without any predefined Test Cases or documentation. The primary objective is to break the application by performing unusual operations and verify whether it remains stable.

Because the tester behaves like a monkey randomly interacting with the application, Adhoc Testing is also known as **Monkey Testing** or **Gorilla Testing**.

---

## Definition

**Adhoc Testing** is a type of software testing in which the Test Engineer performs **abnormal or random actions** on the software with the intention of breaking the system and verifying its stability.

Since abnormal actions are performed on the application, Adhoc Testing is also called **Monkey Testing** or **Gorilla Testing**.

---

## Objectives of Adhoc Testing

Adhoc Testing is performed to:

- **Identify hidden defects.**
- **Check application stability.**
- **Break the application using unexpected actions.**
- **Verify software robustness.**
- **Improve software reliability.**
- **Discover defects not covered by Test Cases.**

---

## Characteristics of Adhoc Testing

- **No predefined Test Cases.**
- **No formal documentation.**
- **Random testing approach.**
- **Based on tester experience and creativity.**
- **Focuses on breaking the application.**
- **Usually performed after Functional Testing.**

---

## Adhoc Testing Workflow

```text
Application Ready
        │
        ▼
Perform Random Actions
        │
        ▼
Observe Application Behavior
        │
   ┌────┴────┐
   │         │
 Stable   Application Fails
   │         │
   ▼         ▼
Pass     Report Defect
```

---

## Adhoc Testing Process

### Step 1 – Understand the Application

The Test Engineer gains a basic understanding of the application functionality.

---

### Step 2 – Perform Random Actions

The Tester performs unexpected operations without following any predefined Test Cases.

Examples include:

- Clicking buttons repeatedly.
- Refreshing the page multiple times.
- Entering invalid data.
- Opening multiple browser tabs.
- Navigating randomly.
- Pressing keyboard shortcuts repeatedly.

---

### Step 3 – Observe the Application

The application's response is carefully observed.

---

### Step 4 – Report Defects

If the application crashes or behaves unexpectedly, the defect is reported.

---

## Example

### Account Blocking Page

```text
-----------------------------------

        Account Blocking

Account Number :

____________________

Comment :

____________________

        [ Block ]

-----------------------------------
```

### Test Scenario

The Test Engineer:

- Pastes the URL of the Account Blocking page directly into the browser.
- Clicks the **Block** button repeatedly.
- Refreshes the page continuously.
- Enters invalid Account Numbers.
- Leaves mandatory fields blank.

### Expected Result

The application should remain stable and should not crash.

If the application handles all abnormal actions correctly, it is considered stable.

---

## Common Adhoc Testing Scenarios

A Test Engineer may perform the following actions:

- Click the Login button multiple times.
- Press the browser Back button repeatedly.
- Refresh the application continuously.
- Enter extremely large input values.
- Paste SQL Injection statements.
- Upload unsupported file types.
- Open multiple browser tabs simultaneously.
- Disconnect the internet while submitting data.
- Use invalid URLs.
- Perform rapid mouse clicks.

---

## Monkey Testing vs Gorilla Testing

Although both terms are often used interchangeably, there is a slight difference.

### Monkey Testing

- Random testing throughout the application.
- Focuses on finding unexpected defects.
- No predefined objective.

### Gorilla Testing

- Repeatedly tests a specific module.
- Focuses on breaking one functionality.
- Performs intensive testing on a single feature.

---

## Adhoc Testing vs Exploratory Testing

| **Adhoc Testing** | **Exploratory Testing** |
|-------------------|-------------------------|
| Random testing. | Learning, testing, and exploration happen together. |
| No planning. | Some planning and learning are involved. |
| Objective is to break the application. | Objective is to discover defects through exploration. |
| No documentation. | Test ideas may be documented. |
| Highly random. | More structured than Adhoc Testing. |

---

## Advantages of Adhoc Testing

- **Identifies hidden defects.**
- **No Test Case preparation required.**
- **Quick to perform.**
- **Improves application stability.**
- **Enhances software reliability.**
- **Useful for experienced Test Engineers.**

---

## Disadvantages of Adhoc Testing

- **No documentation.**
- **Test coverage cannot be measured accurately.**
- **Difficult to reproduce defects if not recorded.**
- **Depends heavily on tester experience.**
- **Not suitable for formal project reporting.**

---

## Real-Time Example

Consider an **Online Banking Application**.

A Test Engineer performs the following abnormal actions:

- Clicks the **Transfer Money** button repeatedly.
- Refreshes the page during a transaction.
- Opens the same account in multiple browser tabs.
- Pastes the transaction URL directly.
- Disconnects the internet while submitting the transaction.

The application should handle all these situations gracefully without crashing or corrupting data.

---

## Frequently Asked Interview Questions

### 1. What is Adhoc Testing?

Adhoc Testing is an informal software testing technique in which the Tester performs random actions to break the application and verify its stability.

---

### 2. Why is Adhoc Testing called Monkey Testing?

Because the Tester performs random and unpredictable actions on the application similar to the behavior of a monkey.

---

### 3. What is the objective of Adhoc Testing?

To identify hidden defects and verify the stability and robustness of the software.

---

### 4. Are Test Cases prepared before Adhoc Testing?

No. Adhoc Testing is performed without predefined Test Cases.

---

### 5. When is Adhoc Testing usually performed?

It is generally performed after Functional Testing when the basic functionality has already been verified.

---

## Key Points

- **Adhoc Testing is an informal testing technique.**
- **It is also known as Monkey Testing or Gorilla Testing.**
- **No Test Cases or documentation are prepared.**
- **The main objective is to break the application and verify its stability.**
- **Experienced Test Engineers are more effective at performing Adhoc Testing.**
- **It helps discover hidden defects that structured testing may miss.**

---

## Summary

**Adhoc Testing** is an informal software testing technique in which Test Engineers perform random and abnormal actions on an application without predefined Test Cases. Its primary objective is to identify hidden defects and evaluate the stability of the software under unexpected conditions. Also known as **Monkey Testing** or **Gorilla Testing**, this approach relies heavily on the tester's experience, creativity, and intuition. Although it is not a replacement for structured testing, Adhoc Testing is highly effective in discovering defects that may remain undetected during regular Functional Testing.
