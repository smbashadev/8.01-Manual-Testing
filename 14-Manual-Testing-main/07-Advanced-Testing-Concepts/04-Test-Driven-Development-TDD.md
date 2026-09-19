# Test Driven Development (TDD)

## Introduction

**Test Driven Development (TDD)** is a software development approach in which developers write test cases **before writing the actual source code**. Instead of writing code first, developers first create a test that describes the expected behavior of the software.

The developer then writes the minimum amount of code required to pass the test. This process is repeated until all functionalities are implemented successfully.

TDD helps improve software quality, reduces defects, and encourages clean, maintainable code.

---

## Definition

**Test Driven Development (TDD)** is a software development methodology in which **test cases are written before writing the actual implementation code**.

The developer repeatedly writes a test, develops the code to satisfy the test, and refactors the code while ensuring that all tests continue to pass.

---

## Objectives of TDD

Test Driven Development is used to:

- **Develop high-quality software.**
- **Reduce software defects.**
- **Improve code design.**
- **Increase code coverage.**
- **Encourage modular programming.**
- **Simplify maintenance.**

---

## TDD Cycle

The Test Driven Development process follows a continuous cycle.

```text
Write Test Case
       │
       ▼
Run Test
       │
       ▼
Test Fails
       │
       ▼
Write Minimum Code
       │
       ▼
Run Test Again
       │
       ▼
Test Passes
       │
       ▼
Refactor Code
       │
       ▼
Repeat
```

---

## TDD Workflow (Based on Classroom Notes)

```text
                 Developer

            Add a Test Case
                   │
                   ▼
              Run the Test
                   │
            (Test Fails)
                   │
                   ▼
          Do a Little Change
           (Write the Code)
                   │
                   ▼
              Run the Test
                   │
            (Test Passes)
                   │
                   ▼
             End of Coding

          Repeat for Every Test Case
```

---

## Steps in Test Driven Development

### Step 1 – Write a Test Case

The Developer writes a Test Case based on the requirement.

Since no implementation exists, the test fails initially.

---

### Step 2 – Run the Test

Execute the newly written Test Case.

The expected result is **Fail** because the functionality has not yet been implemented.

---

### Step 3 – Write the Minimum Code

The Developer writes only the amount of code required to make the failed Test Case pass.

---

### Step 4 – Run the Test Again

Execute the Test Case again.

If the implementation is correct, the Test Case passes.

---

### Step 5 – Refactor the Code

Improve the internal code structure without changing its behavior.

After refactoring, execute all Test Cases again to ensure that everything still works correctly.

---

## TDD Development Flow

```text
Requirement
      │
      ▼
Write Test Case
      │
      ▼
Execute Test
      │
      ▼
Fail
      │
      ▼
Write Code
      │
      ▼
Execute Test
      │
 ┌────┴────┐
 │         │
Pass      Fail
 │         │
 ▼         ▼
Refactor  Modify Code
 │         │
 └────┬────┘
      ▼
Next Requirement
```

---

## Example

Requirement:

```text
Calculate the addition of two numbers.
```

### Step 1

Write the Test Case.

```java
assertEquals(6, add(2,4));
```

The test fails because the method does not exist.

---

### Step 2

Implement the method.

```java
public int add(int a,int b){
    return a+b;
}
```

---

### Step 3

Execute the Test Case again.

Result:

```text
PASS
```

---

### Step 4

Improve the code if necessary.

Run all Test Cases again.

---

## TDD Rules

The three basic rules of TDD are:

1. **Do not write production code until you have written a failing Test Case.**

2. **Write only enough code to make the Test Case pass.**

3. **Refactor the code after all Test Cases pass.**

---

## Common TDD Frameworks

| **Programming Language** | **Framework** |
|---------------------------|---------------|
| Java | JUnit, TestNG |
| Python | PyTest, unittest |
| JavaScript | Jest |
| C# | NUnit |
| C++ | Google Test |

---

## Advantages of TDD

- **Improves software quality.**
- **Reduces software defects.**
- **Provides high code coverage.**
- **Improves code maintainability.**
- **Encourages modular design.**
- **Makes debugging easier.**
- **Supports continuous integration.**
- **Improves developer confidence.**

---

## Disadvantages of TDD

- **Requires additional development time initially.**
- **Developers must have good testing knowledge.**
- **Not suitable for very small projects.**
- **Maintaining Test Cases requires additional effort.**
- **Can slow development if requirements change frequently.**

---

## TDD vs Traditional Development

| **Traditional Development** | **Test Driven Development** |
|------------------------------|-----------------------------|
| Code is written first. | Test Cases are written first. |
| Testing happens after development. | Testing happens throughout development. |
| Bugs are detected later. | Bugs are detected early. |
| Lower code coverage. | Higher code coverage. |
| More debugging effort. | Easier debugging. |

---

## Real-Time Example

Suppose a Developer is implementing the **Login Module** of an Online Banking Application.

Instead of writing the Login code immediately, the Developer first writes Test Cases such as:

- Valid Username and Password
- Invalid Username
- Invalid Password
- Empty Username
- Empty Password

Initially, all Test Cases fail.

The Developer then implements only enough code to satisfy these Test Cases.

After all Test Cases pass, the code is refactored and integrated into the application.

---

## Frequently Asked Interview Questions

### 1. What is Test Driven Development (TDD)?

TDD is a software development methodology in which Test Cases are written before writing the actual implementation code.

---

### 2. Who performs TDD?

**Developers** perform Test Driven Development.

---

### 3. What is the first step in TDD?

Write a **failing Test Case**.

---

### 4. What happens after the Test Case fails?

The Developer writes the minimum amount of code required to make the Test Case pass.

---

### 5. Name some frameworks used for TDD in Java.

- JUnit
- TestNG

---

## Key Points

- **TDD stands for Test Driven Development.**
- **Test Cases are written before writing production code.**
- **Every new feature begins with a failing Test Case.**
- **Only the minimum required code is written.**
- **After the Test passes, the code is refactored.**
- **TDD improves software quality and reduces defects.**

---

## Summary

**Test Driven Development (TDD)** is a software development methodology in which developers write Test Cases before implementing the actual code. The development process follows a continuous cycle of writing a failing Test Case, implementing the minimum required code, executing the test until it passes, and then refactoring the code. TDD helps improve software quality, increase code coverage, reduce defects, and produce clean, maintainable, and reliable software through continuous testing and incremental development.
