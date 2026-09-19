# V-Model (Verification and Validation Model)

## Introduction

The **V-Model**, also known as the **Verification and Validation Model**, is one of the most widely used **Software Development Life Cycle (SDLC)** models. It is an extension of the **Waterfall Model**, where every development phase has a corresponding testing phase.

Unlike the Waterfall Model, testing activities begin from the early stages of software development. This enables the testing team to prepare test plans and test cases well before coding begins, helping identify defects earlier and improving the overall software quality.

The V-Model is best suited for projects where the requirements are clearly defined and are not expected to change during development.

---

## Definition

The **V-Model (Verification and Validation Model)** is a Software Development Life Cycle (SDLC) model in which every software development activity is associated with a corresponding testing activity.

The left side of the model represents the **Verification Phase**, while the right side represents the **Validation Phase**. Both phases meet at the **Coding** stage.

---

## V-Model Workflow

The V-Model establishes a relationship between every development phase and its corresponding testing phase.

```text
Verification Phase                           Validation Phase

CRS ---------------------------------------> Acceptance Testing
   SRS -----------------------------------> System Testing
      HLD -------------------------------> Integration Testing
         LLD ---------------------------> Functional Testing
            Coding --------------------> Unit Testing
                     Code
```

### Abbreviations

- **CRS** – Customer Requirement Specification
- **SRS** – Software Requirement Specification
- **HLD** – High-Level Design
- **LLD** – Low-Level Design

---

## Understanding the Workflow

The V-Model follows two parallel activities:

### Verification Phase

During the Verification Phase, the software is planned and designed.

The development team prepares:

- Customer Requirements
- Software Requirements
- High-Level Design
- Low-Level Design

No software execution takes place during this phase.

---

### Validation Phase

Once coding is completed, the testing team validates every development activity by performing the corresponding testing activity.

The software is executed and verified to ensure it satisfies customer requirements.

---

## What is Verification?

### Definition

**Verification** involves **static analysis techniques** performed **without executing the software code**.

It is the process of evaluating every product development phase to determine whether the specified requirements are correctly implemented.

Verification answers the question:

**"Are we building the product correctly?"**

---

### Verification Activities

Verification mainly includes:

- Requirement Review
- Design Review
- Code Review
- Walkthrough
- Inspection

---

### Characteristics of Verification

- **Static Testing Technique**
- **No program execution**
- **Performed during software development**
- **Detects defects early**
- **Improves software quality**
- **Reduces development cost**

---

## What is Validation?

### Definition

**Validation** involves **dynamic analysis techniques** performed by executing the software.

It is the process of evaluating the completed software to determine whether it satisfies customer expectations and business requirements.

Validation answers the question:

**"Are we building the correct product?"**

---

### Validation Activities

Validation includes:

- Unit Testing
- Functional Testing
- Integration Testing
- System Testing
- Acceptance Testing

---

### Characteristics of Validation

- **Dynamic Testing Technique**
- **Software execution is required**
- **Performed after coding**
- **Validates business requirements**
- **Ensures customer satisfaction**

---

## Relationship Between Verification and Validation

Each development phase has a corresponding testing phase.

| **Verification Activity** | **Validation Activity** |
|---------------------------|-------------------------|
| Customer Requirement Specification (CRS) | Acceptance Testing |
| Software Requirement Specification (SRS) | System Testing |
| High-Level Design (HLD) | Integration Testing |
| Low-Level Design (LLD) | Functional Testing |
| Coding | Unit Testing |

This relationship helps identify defects as early as possible and improves software quality.


## Difference Between Verification and Validation

| **Verification** | **Validation** |
|------------------|----------------|
| Verification is a **static analysis technique**. | Validation is a **dynamic analysis technique**. |
| The software is **not executed** during verification. | The software is **executed** during validation. |
| Ensures the product is developed according to specifications. | Ensures the developed product satisfies customer requirements. |
| Performed during the development phases. | Performed after the development phase. |
| Includes reviews, walkthroughs, and inspections. | Includes Unit Testing, Functional Testing, Integration Testing, System Testing, and Acceptance Testing. |
| Detects defects before software execution. | Detects defects after software execution. |

---

## Advantages of the V-Model

The V-Model offers several benefits for software development projects where requirements are stable and clearly defined.

- **Easy to understand and implement.**
- **Testing activities such as test planning and test case design begin before coding starts.**
- **Early testing saves both development time and cost.**
- **Provides a higher probability of project success compared to the Waterfall Model.**
- **Helps prevent defects from progressing to later development stages.**
- **Suitable for small and medium-sized projects with well-defined requirements.**
- **Improves software quality through early verification and validation.**
- **Each development phase has a corresponding testing phase, making defect tracking easier.**

---

## Disadvantages of the V-Model

Although the V-Model improves software quality, it also has certain limitations.

- **Very rigid and less flexible.**
- **Not suitable for large or complex projects.**
- **Working software is not available until the coding phase is completed.**
- **Requirement changes are difficult to accommodate once development has started.**
- **Any change in requirements requires updates to both development and testing documents.**
- **Customer feedback is received only after implementation.**
- **Not suitable for projects where requirements change frequently.**

---

## Real-Time Example

Consider the development of an **Online Banking Application**.

### Verification Phase

The development team performs the following activities:

- Prepare the **Customer Requirement Specification (CRS)**.
- Create the **Software Requirement Specification (SRS)**.
- Design the software architecture using **High-Level Design (HLD)**.
- Prepare the detailed module design using **Low-Level Design (LLD)**.

These activities are reviewed and verified before development begins.

### Coding Phase

Developers implement the application using the approved design documents.

### Validation Phase

After coding is completed, the testing team performs:

- **Unit Testing** to verify individual modules.
- **Functional Testing** to verify business functionality.
- **Integration Testing** to verify communication between modules.
- **System Testing** to validate the complete application.
- **Acceptance Testing** to ensure the software satisfies customer expectations.

If defects are found, they are reported to developers, fixed, and then re-tested.

---

## When to Use the V-Model

The V-Model is recommended when:

- **Project requirements are fixed and clearly understood.**
- **Requirement changes are very minimal.**
- **Software quality is the highest priority.**
- **Testing needs to be planned from the beginning of the project.**
- **The project is small or medium-sized.**
- **The project involves safety-critical or quality-critical systems.**

---

## Key Points

- **V-Model stands for Verification and Validation Model.**
- **It is an enhancement of the Waterfall Model.**
- **Every development phase has a corresponding testing phase.**
- **Verification uses static testing techniques.**
- **Validation uses dynamic testing techniques.**
- **Testing activities are planned before coding begins.**
- **Early defect detection improves software quality and reduces development cost.**
- **The V-Model is best suited for projects with stable requirements.**

---

## Summary

The **V-Model (Verification and Validation Model)** is a structured Software Development Life Cycle (SDLC) model that emphasizes quality by associating every development activity with a corresponding testing activity. Verification ensures that each development phase satisfies the specified requirements through static analysis, while Validation confirms that the developed software meets customer expectations through dynamic testing. The V-Model is simple, systematic, and highly effective for projects with well-defined requirements where quality assurance is a primary objective.
