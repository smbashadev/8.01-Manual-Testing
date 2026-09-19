## Question 21

### What are the Principles of Software Testing?

Software Testing follows seven fundamental principles that help testers perform effective testing and improve software quality.

### The Seven Principles of Testing

1. Testing shows the presence of defects, not their absence.
2. Exhaustive testing is impossible.
3. Early testing saves time and cost.
4. Defects are clustered together.
5. Beware of the pesticide paradox.
6. Testing depends on the context.
7. Absence of errors is a fallacy.

---

## Question 22

### Explain the First Principle: Testing Shows the Presence of Defects

Testing can reveal defects in software, but it cannot prove that the software is completely free from defects.

**Example**

Even after executing thousands of test cases, some hidden defects may still exist.

---

## Question 23

### What is Exhaustive Testing?

Exhaustive Testing means testing every possible input, condition, and execution path.

In real-world projects, exhaustive testing is impossible because applications have millions of possible combinations.

Therefore, testers use risk-based testing and prioritize important scenarios.

---

## Question 24

### What is Early Testing?

Early Testing means beginning testing activities during the initial stages of software development.

Testing starts from requirement analysis instead of waiting until coding is completed.

**Benefits**

- Detects defects early
- Reduces development cost
- Saves testing effort
- Improves software quality

---

## Question 25

### What is Defect Clustering?

Defect Clustering means that a small number of modules usually contain most of the defects.

This follows the Pareto Principle (80/20 Rule).

**Example**

80% of bugs are often found in 20% of the application's modules.

---

## Question 26

### What is the Pesticide Paradox?

Executing the same test cases repeatedly eventually stops finding new defects.

To discover new defects, testers should regularly update and improve their test cases.

---

## Question 27

### What is Context-Dependent Testing?

Testing methods vary depending on the type of application.

**Examples**

- Banking applications require security testing.
- Medical software requires accuracy testing.
- Gaming applications require performance testing.
- E-commerce applications require usability testing.

---

## Question 28

### What is the Absence of Errors Fallacy?

Even if software has no known defects, it can still fail if it does not satisfy customer requirements.

Bug-free software that does not meet business needs is considered unsuccessful.

---

## Question 29

### What is a Test Scenario?

A Test Scenario is a high-level description of a functionality that needs to be tested.

It identifies **what** should be tested without describing detailed steps.

**Example**

Verify user login functionality.

---

## Question 30

### What is a Test Case?

A Test Case is a detailed document containing steps, input data, expected results, and actual results used to verify a specific functionality.

### Components of a Test Case

- Test Case ID
- Test Scenario
- Preconditions
- Test Steps
- Test Data
- Expected Result
- Actual Result
- Status

---

## Question 31

### What is the Difference Between Test Scenario and Test Case?

| Test Scenario | Test Case |
|--------------|-----------|
| High-level description | Detailed testing document |
| Describes what to test | Describes how to test |
| Covers functionality | Covers execution steps |
| Less detailed | Highly detailed |

---

## Question 32

### What is a Test Suite?

A Test Suite is a collection of multiple related test cases grouped together for execution.

**Example**

Login Test Suite may contain:

- Valid Login
- Invalid Login
- Empty Username
- Empty Password
- Forgot Password
- Locked User

---

## Question 33

### What is Test Data?

Test Data is the input provided to execute test cases.

It may include valid, invalid, boundary, or random values.

**Example**

Username: admin

Password: Admin@123

---

## Question 34

### What is RTM (Requirement Traceability Matrix)?

Requirement Traceability Matrix (RTM) is a document that maps requirements with corresponding test cases.

It ensures every requirement is tested.

### Benefits

- Requirement coverage
- Easy tracking
- Missing test case identification
- Requirement verification

---

## Question 35

### What is Requirement Coverage?

Requirement Coverage measures how completely software requirements are tested.

A project is considered well tested when every requirement has at least one associated test case.

---

## Question 36

### What is a Defect Life Cycle?

The Defect Life Cycle represents the stages through which a defect passes from discovery until closure.

### Common Stages

- New
- Assigned
- Open
- Fixed
- Retest
- Verified
- Closed

Additional stages may include:

- Reopened
- Deferred
- Rejected
- Duplicate
- Cannot Reproduce

---

## Question 37

### Explain the Defect Statuses

**New**

The tester reports a defect.

**Assigned**

The defect is assigned to a developer.

**Open**

Developer begins investigating the issue.

**Fixed**

Developer fixes the defect.

**Retest**

Tester verifies the fix.

**Verified**

Tester confirms the issue is resolved.

**Closed**

The defect is officially closed.

---

## Question 38

### What is Severity?

Severity indicates how serious the impact of a defect is on the application's functionality.

### Severity Levels

- Critical
- High
- Medium
- Low

Severity is usually determined by the tester.

---

## Question 39

### What is Priority?

Priority indicates how quickly a defect should be fixed.

### Priority Levels

- High
- Medium
- Low

Priority is generally decided by the Project Manager, Product Owner, or Business Analyst.

---

## Question 40

### What is the Difference Between Severity and Priority?

| Severity | Priority |
|----------|----------|
| Measures impact | Measures urgency |
| Decided by tester | Decided by business or project team |
| Technical perspective | Business perspective |
| Indicates seriousness | Indicates fix order |

### Example

A company logo displayed incorrectly on the homepage:

- Severity: Low
- Priority: High

Reason: It does not affect functionality but impacts the company's public image.

---

# End of Part 2 (Questions 21–40)

**Part 3 (Questions 41–60) will cover:**

- Smoke Testing
- Sanity Testing
- Regression Testing
- Retesting
- Functional Testing
- Non-Functional Testing
- Black Box Testing
- White Box Testing
- Gray Box Testing
- Static Testing
- Dynamic Testing
- Ad-hoc Testing
- Exploratory Testing
- Monkey Testing
- Gorilla Testing
- Positive & Negative Testing
- End-to-End Testing
- Integration Testing
- System Testing
- Acceptance Testing
