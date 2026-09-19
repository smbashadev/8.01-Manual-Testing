# Waterfall Model

## Introduction

The **Waterfall Model** is one of the earliest and most widely used **Software Development Life Cycle (SDLC)** models. It follows a **linear and sequential approach**, where each phase must be completed before moving to the next phase.

In the Waterfall Model, the output of one phase becomes the input for the next phase. Since every phase is completed one after another, it resembles the flow of a waterfall, which is why it is called the **Waterfall Model**.

The Waterfall Model is **documentation-intensive**, meaning every phase produces documents that guide the activities of the subsequent phases.

## Definition

The **Waterfall Model** is a linear Software Development Life Cycle (SDLC) model in which the software development process is divided into multiple sequential phases. Each phase must be completed before the next phase begins, and the output of one phase serves as the input for the following phase.

## Waterfall Model Diagram

> **Note:** Replace the diagram below with the Waterfall Model image provided by your trainer if you want to use the original classroom diagram.

```text
Customer Requirements (CRS)
            │
            ▼
Requirement Gathering & Analysis
            │
            ▼
     Feasibility Study
            │
            ▼
          Design
     (HLD & LLD)
            │
            ▼
          Coding
            │
            ▼
          Testing
            │
            ▼
 Installation / Deployment
            │
            ▼
       Maintenance
```

## Important Terminologies

| **Term** | **Full Form** |
|-----------|---------------|
| **CRS** | Customer Requirement Specification |
| **SRS** | Software Requirement Specification |
| **HLD** | High-Level Design |
| **LLD** | Low-Level Design |
| **BA** | Business Analyst |
| **PA** | Product Analyst |

## Phases of the Waterfall Model

### 1. Requirement Gathering and Analysis

This is the first phase of the Waterfall Model.

The **Business Analyst (BA)** or **Product Analyst (PA)** interacts with the customer to gather all the business requirements.

After gathering the requirements, they are carefully analyzed to identify:

- **Incomplete requirements**
- **Inconsistent requirements**
- **Conflicting requirements**
- **Missing requirements**

The objective of this phase is to prepare a clear and complete **Customer Requirement Specification (CRS)** document.

### 2. Feasibility Study

After the requirements are finalized, a feasibility study is conducted.

The purpose of this phase is to determine whether developing the software is practical and achievable.

The project is analyzed based on:

- **Technical Feasibility**
- **Economic Feasibility**
- **Operational Feasibility**
- **Legal Feasibility**
- **Schedule Feasibility**

Different solution strategies are evaluated, and the most suitable approach is selected for implementation.

### 3. Design

During this phase, the **Software Requirement Specification (SRS)** is converted into a software design.

The Design Engineer prepares:

### High-Level Design (HLD)

HLD describes:

- **Overall system architecture**
- **Major modules**
- **Module relationships**
- **Database architecture**
- **Technology stack**

### Low-Level Design (LLD)

LLD describes:

- **Detailed module logic**
- **Flowcharts**
- **Database tables**
- **Input and output design**
- **Error handling**
- **Interface details**

The design document acts as the blueprint for software development.

### 4. Coding

After the design is completed, developers begin writing the source code.

During this phase:

- **Each module is developed separately.**
- **Coding standards are followed.**
- **Programming languages and development tools are used to implement the design.**

This is generally the longest phase of software development.

### 5. Testing

Once coding is completed, the software is handed over to the **Testing Team**.

The **QA Engineers (Test Engineers)** execute test cases to verify that the software functions according to the customer requirements.

If defects are found:

- **They are reported to the development team.**
- **Developers fix the defects.**
- **The application is re-tested until it becomes stable.**

### 6. Installation / Deployment

After successful testing, the software is deployed to the customer's environment or released to the production server.

The Installation Engineer verifies that the application works correctly after deployment.

### 7. Maintenance

Maintenance begins once the software is delivered to the customer.

It includes:

- **Bug Fixing**
- **Software Upgrades**
- **Feature Enhancements**
- **Performance Improvements**

Maintenance continues throughout the software's operational life.

## Advantages of the Waterfall Model

- **Simple and easy to understand.**
- **Easy to implement and manage.**
- **Clearly defined development phases.**
- **Well-organized documentation.**
- **Easy to monitor project progress.**
- **Suitable for projects with stable and well-defined requirements.**
- **Works well for small and medium-sized projects.**

## Disadvantages of the Waterfall Model

- **Working software is available only after the development phase is completed.**
- **Requirement changes are difficult to implement.**
- **High project risk if requirements change frequently.**
- **Not suitable for large or complex projects.**
- **Testing begins only after coding is completed.**
- **Customer feedback is received late in the development process.**

## Real-Time Example

Suppose a college wants to develop a **Student Management System**.

The requirements are fixed before development begins.

The development team proceeds through the following phases:

- **Requirement Analysis**
- **Feasibility Study**
- **Design**
- **Coding**
- **Testing**
- **Deployment**
- **Maintenance**

Since the requirements are stable and unlikely to change, the **Waterfall Model** is an appropriate choice.

## When to Use the Waterfall Model

The Waterfall Model is suitable when:

- **Project requirements are clear and fixed.**
- **The project is small or medium-sized.**
- **Technology is well understood.**
- **Frequent requirement changes are not expected.**
- **Detailed documentation is required.**

## Key Points

- **The Waterfall Model is a sequential SDLC model.**
- **Each phase must be completed before moving to the next phase.**
- **The output of one phase becomes the input for the next phase.**
- **It is a documentation-driven software development model.**
- **It is best suited for projects with stable requirements.**

## Summary

The **Waterfall Model** is one of the most popular Software Development Life Cycle models that follows a sequential approach to software development. Every phase is completed one after another, ensuring proper planning, documentation, and execution. Although it is simple and easy to manage, it is most effective when project requirements are well understood and are unlikely to change during development.
