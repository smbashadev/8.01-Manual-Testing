# White Box Testing

## Introduction

**White Box Testing** is a software testing technique that verifies the internal working structure of a software application. Unlike Black Box Testing, the tester has complete knowledge of the application's source code, program logic, control flow, conditions, loops, and execution paths.

White Box Testing ensures that every important statement, path, loop, and condition in the source code is executed and verified. It helps identify logical errors, unreachable code, coding mistakes, and security vulnerabilities before the software is delivered to the customer.

This testing technique is generally performed by developers or testers who have programming knowledge.

---

## Definition

**White Box Testing** is a software testing technique in which the internal code structure, implementation details, logic, conditions, loops, and execution paths of a software application are verified.

The tester has complete knowledge of the application's source code and designs test cases to verify the correctness of the program logic.

White Box Testing is also known as:

- **Structural Testing**
- **Code-Based Testing**
- **Glass Box Testing**
- **Clear Box Testing**
- **Open Box Testing**
- **Transparent Box Testing**

---

## Characteristics of White Box Testing

The following are the important characteristics of White Box Testing:

- **Requires programming knowledge.**
- **Focuses on internal source code and logic.**
- **Verifies statements, conditions, paths, and loops.**
- **Helps improve code quality.**
- **Identifies logical errors early.**
- **Ensures maximum code coverage.**
- **Detects unreachable (dead) code.**

---

## Advantages of White Box Testing

- **Improves software quality.**
- **Detects logical and coding errors.**
- **Provides better code coverage.**
- **Helps identify security vulnerabilities.**
- **Detects unreachable code.**
- **Improves application performance.**
- **Facilitates easier debugging.**

---

## Disadvantages of White Box Testing

- **Requires programming knowledge.**
- **Time-consuming for large applications.**
- **Complete code coverage may be difficult.**
- **Frequent code changes require repeated testing.**
- **Not suitable for validating business requirements alone.**

---

## Types of White Box Testing

White Box Testing mainly consists of the following types:

1. **Statement Testing**
2. **Loop Testing**
3. **Path Testing**
4. **Conditional Testing**

---

# 1. Statement Testing

## Definition

**Statement Testing** is a type of White Box Testing in which the Test Engineer applies one or more test cases to verify whether every executable statement in the program is executed at least once.

The objective of Statement Testing is to ensure that every executable statement is covered during testing.

---

## Java Program

```java
package Testing;

import java.util.Scanner;

public class Demo {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.println("Please enter a number : ");

        int num = sc.nextInt();

        switch(num)
        {
            case 1:
                System.out.println("You have entered 1");
                break;

            case 2:
                System.out.println("You have entered 2");
                break;

            case 3:
                System.out.println("You have entered 3");
                break;

            default:
                System.out.println("Please check the output statement once before entering any number");
                break;
        }
    }
}
```

---

## Explanation

The above program accepts an integer from the user and executes one of the available **switch-case** statements.

To achieve **Statement Coverage**, the tester must execute every possible executable statement at least once.

This requires designing multiple test cases.

---

## Sample Test Cases

| **Test Case ID** | **Input** | **Procedure** | **Expected Output** | **Actual Output** | **Result** |
|------------------|-----------|---------------|---------------------|-------------------|------------|
| **STT-01** | num = 1 | Execute the program by entering **1**. | "You have entered 1" should be displayed. | Same as Expected. | **Pass** |
| **STT-02** | num = 2 | Execute the program by entering **2**. | "You have entered 2" should be displayed. | Same as Expected. | **Pass** |
| **STT-03** | num = 3 | Execute the program by entering **3**. | "You have entered 3" should be displayed. | Same as Expected. | **Pass** |
| **STT-04** | num = 45 | Execute the program by entering **45**. | Default message should be displayed. | Same as Expected. | **Pass** |

---

## Statement Coverage

Statement Coverage measures how many executable statements are executed during testing.

### Formula

```text
Statement Coverage (Cs)

Cs = (Number of Statements Executed / Total Number of Statements) × 100
```

---

## Statement Coverage Example

Consider the following Java program.

```java
package Testing;

import java.util.Scanner;

public class Demo1 {

    void add() {

        Scanner sc = new Scanner(System.in);

        System.out.println("Please enter a value for a : ");

        int a = sc.nextInt();

        System.out.println("Please enter a value for b : ");

        int b = sc.nextInt();

        int add = a + b;

        System.out.println("Addition Result : " + add);
    }

    void sub(int a, int b) {

        int sub = a - b;

        System.out.println("Subtraction Result : " + sub);
    }

    void mul() {

        Scanner sc = new Scanner(System.in);

        System.out.println("Please enter a value for a : ");

        int a = sc.nextInt();

        System.out.println("Please enter a value for b : ");

        int b = sc.nextInt();

        int mul = a * b;

        System.out.println("Multiplication Result : " + mul);
    }

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        Demo1 d = new Demo1();

        d.add();

        System.out.println("Values for Subtraction");

        System.out.println("Please enter a value for a : ");

        int a = sc.nextInt();

        System.out.println("Please enter a value for b : ");

        int b = sc.nextInt();

        d.sub(a, b);
    }
}
```

---

## Infeasible Statements

In the above program, the **mul()** method is never invoked from the **main()** method.

Therefore, all executable statements inside the **mul()** method are **never executed**.

Such statements are known as **Infeasible Statements**.

### Definition

**Infeasible Statements** are executable statements that can never be executed because there is no execution path that reaches them during program execution.

Identifying infeasible statements helps improve code quality and remove unnecessary or unreachable code.

---

## Key Points

- **Statement Testing verifies executable statements.**
- **Every executable statement should execute at least once.**
- **Statement Coverage measures the percentage of executed statements.**
- **Infeasible Statements reduce code coverage.**
- **Higher Statement Coverage generally improves software quality.**


# 2. Path Testing

## Definition

**Path Testing** is a type of **White Box Testing** in which the Test Engineer applies one or more test cases on the **Control Flow Diagram (CFG)** to verify whether every independent execution path in the program is executed at least once.

The objective of Path Testing is to ensure that every possible execution path in the application is tested.

---

## Java Program

```java
package Testing;

import java.util.Scanner;

public class Demo2 {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.println("Please enter the first number : ");

        int num1 = sc.nextInt();

        System.out.println("Please enter the second number : ");

        int num2 = sc.nextInt();

        if(num1 > num2)
        {
            System.out.println("First number is greater");
        }
        else
        {
            System.out.println("Second number is greater");
        }
    }
}
```

---

## Explanation

The above program compares two numbers.

Depending on the condition:

```text
num1 > num2
```

the program follows one of the execution paths.

Path Testing ensures that every execution path is executed at least once.

---

## Control Flow Diagram (CFG)

```text
             ┌──────────────┐
             │    START     │
             └──────┬───────┘
                    │
                    ▼
          Read num1 and num2
                    │
                    ▼
          Is num1 > num2 ?
             /             \
          Yes               No
           │                 │
           ▼                 ▼
Print "First        Print "Second
Number is Greater" Number is Greater"
           │                 │
           └───────┬─────────┘
                   ▼
                STOP
```

---

## Execution Paths

### Path 1

```text
Start
   │
Read num1, num2
   │
num1 > num2
   │
YES
   │
Print First Number is Greater
   │
Stop
```

---

### Path 2

```text
Start
   │
Read num1, num2
   │
num1 > num2
   │
NO
   │
Print Second Number is Greater
   │
Stop
```

---

## Sample Test Cases

| **Test Case ID** | **Input** | **Procedure** | **Expected Output** | **Actual Output** | **Result** |
|------------------|-----------|---------------|---------------------|-------------------|------------|
| **PT-01** | a = 9<br>b = 8 | Execute the program. | First Number is Greater | Same as Expected | **Pass** |
| **PT-02** | a = 11<br>b = 13 | Execute the program. | Second Number is Greater | Same as Expected | **Pass** |
| **PT-03** | a = -11<br>b = -11 | Execute the program. | Second Number is Greater | Same as Expected | **Pass** |

---

## Path Coverage Formula

Path Coverage measures how many execution paths have been covered during testing.

### Formula

```text
Path Coverage (Cp)

Cp = (Number of Paths Covered / Total Number of Paths) × 100
```

---

## Advantages of Path Testing

- **Ensures every execution path is verified.**
- **Improves code quality.**
- **Detects logical errors.**
- **Provides better code coverage than Statement Testing.**
- **Helps identify unreachable paths.**

---

# 3. Loop Testing

## Definition

**Loop Testing** is a type of **White Box Testing** in which the Test Engineer applies one or more test cases on looping constructs to verify whether loops execute correctly under different conditions.

Loop Testing mainly verifies the following three conditions:

1. **Loop should execute exactly once.**
2. **Loop should execute more than once.**
3. **Loop should fail (execute zero times).**

---

## Java Program

```java
package Testing;

import java.util.Scanner;

public class Demo3 {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.println("Please enter a number : ");

        int num = sc.nextInt();

        while(num < 8)
        {
            System.out.println("KodNest");
            num++;
        }

    }
}
```

---

## Explanation

The loop executes only when:

```text
num < 8
```

The Test Engineer designs test cases to verify all possible loop execution scenarios.

---

## Sample Test Cases

| **Test Case ID** | **Input** | **Procedure** | **Expected Output** | **Actual Output** | **Result** |
|------------------|-----------|---------------|---------------------|-------------------|------------|
| **LT-01** | num = 7 | Execute the program. | Loop should execute exactly once. | Same as Expected | **Pass** |
| **LT-02** | num = 5 | Execute the program. | Loop should execute more than once. | Same as Expected | **Pass** |
| **LT-03** | num = 1000 | Execute the program. | Loop should not execute. | Same as Expected | **Pass** |

---

## Loop Execution Scenarios

### Case 1

```text
Input : 7

Condition

7 < 8

TRUE

Loop executes exactly once.
```

---

### Case 2

```text
Input : 5

Condition

5 < 8

TRUE

Loop executes multiple times.

5
6
7

Loop Stops.
```

---

### Case 3

```text
Input : 1000

Condition

1000 < 8

FALSE

Loop does not execute.
```

---

## Exception in do-while Loop

The **do-while loop** is an exception because the loop body executes **at least once**, regardless of the condition.

Therefore, during Loop Testing of a **do-while loop**, only the following conditions are verified:

1. **Loop executes exactly once.**
2. **Loop executes more than once.**

The condition **"Loop should fail"** is not applicable because the do-while loop always executes once before checking the condition.

---

## Advantages of Loop Testing

- **Validates loop execution.**
- **Detects infinite loops.**
- **Improves program reliability.**
- **Ensures proper loop termination.**
- **Verifies boundary conditions.**

# 4. Conditional Testing

## Definition

**Conditional Testing** is a type of **White Box Testing** in which the Test Engineer applies one or more test cases on **simple or complex conditional statements** to verify whether every possible **truth value** is executed at least once.

The primary objective of Conditional Testing is to ensure that every possible condition evaluates correctly and produces the expected result.

---

## Objectives of Conditional Testing

Conditional Testing helps to:

- **Verify every conditional statement in the program.**
- **Ensure all possible truth values are executed.**
- **Detect logical errors in decision-making statements.**
- **Improve code reliability.**
- **Increase code coverage.**

---

## Types of Conditional Statements

Conditional statements are mainly classified into two types:

1. **Simple Conditional Statements**
2. **Complex Conditional Statements**

---

# Simple Conditional Statement

A **Simple Conditional Statement** contains only one logical condition.

### Example

```java
if(a > b)
{
    System.out.println("A is Greater");
}
```

Condition:

```text
(a > b)
```

---

## Truth Values

### Case 1

```text
a = 4
b = 2

Condition

4 > 2

Result

TRUE
```

---

### Case 2

```text
a = 2
b = 4

Condition

2 > 4

Result

FALSE
```

The combination of **TRUE** and **FALSE** outcomes is called the **Truth Value**.

---

# Complex Conditional Statement

A **Complex Conditional Statement** contains two or more logical conditions connected using logical operators such as:

- **&& (AND)**
- **|| (OR)**
- **! (NOT)**

---

## Example 1

```java
(a > b) && (b > c)
```

### Case 1

```text
a = 3
b = 2
c = 1

(3 > 2) && (2 > 1)

TRUE && TRUE

Result

TRUE
```

---

### Case 2

```text
a = 1
b = 2
c = 3

(1 > 2) && (2 > 3)

FALSE && FALSE

Result

FALSE
```

---

## Example 2

```java
(a > b) && (b > c) && (c > a)
```

### Case 1

```text
a = 3
b = 2
c = 1

(3 > 2)
&&
(2 > 1)
&&
(1 > 3)

TRUE
&&
TRUE
&&
FALSE

Final Result

FALSE
```

---

### Case 2

```text
a = 5
b = 5
c = 5

(5 > 5)
&&
(5 > 5)
&&
(5 > 5)

FALSE
&&
FALSE
&&
FALSE

Final Result

FALSE
```

---

## Infeasible Truth Value

### Definition

Sometimes a particular combination of **TRUE** and **FALSE** can never occur because of the program logic.

Such truth values are known as **Infeasible Truth Values**.

### Example

```text
(a > b)
&&
(b > c)
&&
(c > a)
```

No input values can satisfy all three conditions simultaneously.

Therefore, this combination is called an **Infeasible Truth Value**.

---

## Advantages of Conditional Testing

- **Validates decision-making statements.**
- **Improves logical correctness.**
- **Detects incorrect conditional expressions.**
- **Improves software reliability.**
- **Provides better decision coverage.**
- **Helps identify infeasible conditions.**

---

## Disadvantages of Conditional Testing

- **Time-consuming for complex applications.**
- **Large number of test cases may be required.**
- **Complex logical expressions are difficult to analyze.**
- **Complete condition coverage is sometimes impractical.**

---

## Real-Time Example

Consider an **ATM Application**.

The withdrawal process depends on the following condition:

```java
if(balance >= withdrawalAmount)
{
    Withdraw Amount
}
else
{
    Display "Insufficient Balance"
}
```

### Test Case 1

```text
Balance = ₹5000

Withdrawal = ₹2000

Condition

5000 >= 2000

TRUE

Withdrawal Successful
```

---

### Test Case 2

```text
Balance = ₹1000

Withdrawal = ₹5000

Condition

1000 >= 5000

FALSE

Display

Insufficient Balance
```

Conditional Testing verifies both possible outcomes.

---

## Difference Between Statement Testing, Path Testing, Loop Testing and Conditional Testing

| **Testing Type** | **Focus** | **Objective** |
|------------------|-----------|---------------|
| **Statement Testing** | Statements | Execute every executable statement at least once. |
| **Path Testing** | Execution Paths | Execute every independent path at least once. |
| **Loop Testing** | Loop Constructs | Verify loop execution under different conditions. |
| **Conditional Testing** | Decision Statements | Verify every possible truth value. |

---

## Frequently Asked Interview Questions

### 1. What is White Box Testing?

White Box Testing is a software testing technique that verifies the internal code structure, logic, conditions, loops, and execution paths of an application.

---

### 2. Who performs White Box Testing?

Generally, **Developers** or **Test Engineers** having programming knowledge perform White Box Testing.

---

### 3. Name the four major types of White Box Testing.

- **Statement Testing**
- **Path Testing**
- **Loop Testing**
- **Conditional Testing**

---

### 4. What is Statement Coverage?

Statement Coverage measures the percentage of executable statements covered during testing.

Formula:

```text
Cs = (Executed Statements / Total Statements) × 100
```

---

### 5. What is Path Coverage?

Path Coverage measures the percentage of execution paths covered during testing.

Formula:

```text
Cp = (Covered Paths / Total Paths) × 100
```

---

### 6. What is an Infeasible Statement?

An **Infeasible Statement** is a statement that can never be executed because no execution path reaches it.

---

### 7. What is an Infeasible Truth Value?

An **Infeasible Truth Value** is a logical condition that can never become TRUE because of the program's logic.

---

## Key Points

- **White Box Testing verifies the internal structure of a program.**
- **Programming knowledge is required.**
- **Statement Testing verifies executable statements.**
- **Path Testing verifies execution paths.**
- **Loop Testing validates loop behavior.**
- **Conditional Testing verifies truth values.**
- **Statement Coverage and Path Coverage help measure code coverage.**
- **Infeasible Statements and Infeasible Truth Values help identify unreachable code and impossible logical conditions.**

---

## Summary

**White Box Testing** is a software testing technique that focuses on validating the internal logic and implementation of an application. It includes **Statement Testing**, **Path Testing**, **Loop Testing**, and **Conditional Testing**, each designed to verify different aspects of the program's execution. White Box Testing improves code quality, increases code coverage, detects logical errors, and helps developers deliver reliable software by ensuring that statements, paths, loops, and conditional expressions function correctly.
