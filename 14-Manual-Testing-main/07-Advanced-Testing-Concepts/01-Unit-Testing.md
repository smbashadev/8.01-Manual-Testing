# Unit Testing

## Introduction

Unit Testing is the first level of software testing performed during the software development process. It focuses on testing individual units or components of a software application independently to ensure that each unit performs its intended functionality correctly.

A **unit** is the smallest testable part of a software application, such as a method, function, class, or module.

Unit Testing helps developers identify defects at an early stage, making bug fixing easier and reducing the overall development cost.

---

## Definition

**Unit Testing** is a type of software testing in which individual units or components of a software application are tested independently.

The main purpose of Unit Testing is to validate that each unit of software code performs as expected.

Unit Testing is performed during the **Development (Coding) Phase** by **Developers**.

---

## Objectives of Unit Testing

Unit Testing is performed to:

- **Verify individual methods or functions.**
- **Detect defects during development.**
- **Improve code quality.**
- **Simplify debugging.**
- **Reduce software maintenance cost.**
- **Increase developer confidence before integration.**

---

## Characteristics of Unit Testing

- **Tests individual units of code.**
- **Performed by Developers.**
- **Executed during the Coding Phase.**
- **Mostly automated using testing frameworks.**
- **Detects defects at an early stage.**
- **Forms the foundation for Integration Testing.**

---

## What is a Unit?

A **Unit** is the smallest testable component of a software application.

Examples include:

- Method
- Function
- Procedure
- Class
- Component

---

## Unit Testing Workflow

```text
Write Source Code
        │
        ▼
Identify Individual Unit
        │
        ▼
Write Unit Test
        │
        ▼
Execute Unit Test
        │
   ┌────┴────┐
   │         │
 Pass      Fail
   │         │
   ▼         ▼
Next Unit  Fix Code
               │
               ▼
        Execute Again
```

---

## Unit Testing Process

The Unit Testing process generally follows these steps:

### Step 1 – Develop the Code

The Developer writes the program or module.

---

### Step 2 – Identify Units

Individual methods or functions are selected for testing.

---

### Step 3 – Prepare Test Data

Valid and invalid input values are prepared.

---

### Step 4 – Execute Unit Tests

Each unit is executed independently.

---

### Step 5 – Compare Results

The Actual Output is compared with the Expected Output.

---

### Step 6 – Fix Defects

If any defects are identified, the Developer fixes the code and performs Unit Testing again.

---

## Example Program

```java
package Practice;

public class Practice26 {

    static int add(int a, int b) {
        int c = a + b;
        return c;
    }

    int mul(int a, int b) {
        int c = a * b;
        return c;
    }

    public static void main(String[] args) {

        int a = 2;
        int b = 4;

        int c = a + b;
        System.out.println(c);

        int res = a * b;
        System.out.println(res);

        System.out.println(add(a, b));
    }
}
```

---

## Units Present in the Program

The above program contains the following units:

- **add() Method**
- **mul() Method**
- **main() Method**

Each method can be tested independently.

---

## Sample Unit Test Cases

### Testing add() Method

| **Test Case ID** | **Input** | **Expected Output** | **Status** |
|------------------|-----------|---------------------|------------|
| UT-01 | add(2,4) | 6 | Pass |
| UT-02 | add(-2,5) | 3 | Pass |
| UT-03 | add(0,0) | 0 | Pass |

---

### Testing mul() Method

| **Test Case ID** | **Input** | **Expected Output** | **Status** |
|------------------|-----------|---------------------|------------|
| UT-04 | mul(2,4) | 8 | Pass |
| UT-05 | mul(-2,4) | -8 | Pass |
| UT-06 | mul(0,10) | 0 | Pass |

---

## Unit Testing Tools

Some commonly used Unit Testing tools include:

| **Programming Language** | **Tool / Framework** |
|---------------------------|----------------------|
| Java | JUnit, TestNG |
| Python | PyTest, unittest |
| JavaScript | Jest, Mocha |
| C# | NUnit |
| C++ | Google Test |

---

## Advantages of Unit Testing

- **Detects defects early.**
- **Improves code quality.**
- **Makes debugging easier.**
- **Reduces development cost.**
- **Simplifies maintenance.**
- **Improves software reliability.**
- **Supports code refactoring.**
- **Increases developer confidence.**

---

## Disadvantages of Unit Testing

- **Requires additional development time.**
- **Cannot identify Integration defects.**
- **Cannot validate complete system behavior.**
- **Requires good programming knowledge.**
- **Test Cases must be maintained as the code changes.**

---

## Real-Time Example

Consider an **Online Banking Application**.

The Developer writes the following methods:

- Login Validation
- Balance Calculation
- Interest Calculation
- Fund Transfer Validation

Before integrating these modules, each method is tested independently using Unit Testing to ensure it produces the expected output.

Only after successful Unit Testing are the modules integrated with the rest of the application.

---

## Unit Testing vs Integration Testing

| **Unit Testing** | **Integration Testing** |
|------------------|-------------------------|
| Tests individual units. | Tests interaction between modules. |
| Performed by Developers. | Performed by Test Engineers or Developers. |
| Executed during Coding Phase. | Executed after Unit Testing. |
| Detects coding defects. | Detects interface defects. |
| Focuses on individual methods or functions. | Focuses on data flow between modules. |

---

## Frequently Asked Interview Questions

### 1. What is Unit Testing?

Unit Testing is a software testing technique in which individual units or components are tested independently to verify that they work correctly.

---

### 2. Who performs Unit Testing?

**Developers** perform Unit Testing.

---

### 3. During which SDLC phase is Unit Testing performed?

During the **Coding (Development) Phase**.

---

### 4. Name some Unit Testing frameworks for Java.

- **JUnit**
- **TestNG**

---

### 5. What is the main objective of Unit Testing?

To verify that every individual unit of software works as expected before Integration Testing begins.

---

## Key Points

- **Unit Testing is the first level of software testing.**
- **It tests individual methods, functions, or classes.**
- **Developers perform Unit Testing during the Coding Phase.**
- **It helps detect defects early and improves code quality.**
- **Unit Testing forms the foundation for Integration Testing.**

---

## Summary

**Unit Testing** is a software testing technique in which individual units or components of an application are tested independently during the development phase. It is primarily performed by developers to verify that each unit behaves according to its expected functionality. By identifying defects early, Unit Testing improves code quality, simplifies debugging, reduces maintenance costs, and provides a strong foundation for subsequent testing phases such as Integration Testing and System Testing.
