# Prototype Model

## Introduction

The **Prototype Model** is one of the most popular Software Development Life Cycle (SDLC) models used when the project requirements are **not clearly defined** or are expected to change frequently. Instead of directly developing the final software, a working model called a **prototype** is created to understand customer requirements and gather feedback.

The prototype is continuously refined based on customer suggestions until the customer is satisfied. Once the prototype is approved, it serves as the foundation for developing the final software product.

The Prototype Model follows an **iterative approach**, allowing continuous communication between the customer and the development team, thereby reducing misunderstandings and improving software quality.

## Definition

The **Prototype Model** is a Software Development Life Cycle (SDLC) model in which a preliminary version of the software, known as a **prototype**, is developed, tested, and repeatedly refined until it satisfies the customer's requirements.

After customer approval, the prototype becomes the basis for developing the final software application.

This model is most suitable when the project requirements are not completely understood at the beginning of the development process.

## Prototype Model Workflow

```text
Initial Requirements
        │
        ▼
Requirement Analysis
        │
        ▼
Quick Design
        │
        ▼
Build Prototype
        │
        ▼
Customer Evaluation
        │
        ▼
Review and Refinement
        │
        ├───────────────┐
        │               │
        │ Customer Not  │
        │   Satisfied   │
        │               │
        └───────▲───────┘
                │
                ▼
Customer Satisfied
        │
        ▼
Development
        │
        ▼
Testing
        │
        ▼
Deployment
        │
        ▼
Maintenance
```

## Phases of the Prototype Model

The Prototype Model consists of the following phases:

1. Requirement Gathering and Analysis
2. Quick Design
3. Build a Prototype
4. Initial User Evaluation
5. Refining the Prototype
6. Product Development
7. Testing
8. Deployment
9. Maintenance

## Phase 1: Requirement Gathering and Analysis

### Description

The Prototype Model begins with gathering and analyzing customer requirements.

Since the customer may not know all the requirements initially, the development team communicates closely with the customer to understand the expected functionality of the software.

During this phase:

- Customer requirements are collected.
- Business objectives are identified.
- Existing systems are analyzed.
- User expectations are understood.
- Initial project scope is defined.

The collected information serves as the foundation for creating the first prototype.

---

## Phase 2: Quick Design

### Description

After gathering the requirements, a simple design of the application is prepared.

This design is **not the final design**.

Instead, it provides a basic understanding of:

- User Interface (UI)
- Navigation
- Module Structure
- Overall Workflow

The objective is to give the customer an early visualization of how the software will look and function.

The Quick Design phase helps developers build the first working prototype more efficiently.

---

## Phase 3: Build a Prototype

### Description

Based on the Quick Design, developers build a working prototype.

The prototype is **not the complete software application**.

Instead, it demonstrates the important functionalities that allow customers to understand the system.

The prototype may contain:

- Login Page
- Home Page
- Navigation Screens
- Basic Functionalities
- Sample Reports

The primary goal is to collect customer feedback before investing significant time in developing the complete system.

---

## Phase 4: Initial User Evaluation

### Description

The developed prototype is presented to the customer for evaluation.

The customer reviews:

- User Interface
- Navigation
- Features
- Functionality
- Overall User Experience

During this stage, customers provide:

- Suggestions
- Comments
- Corrections
- Additional Requirements

This feedback helps developers understand whether the software meets customer expectations.

---

## Phase 5: Refining the Prototype

### Description

If the customer is not satisfied with the prototype, the development team modifies it according to the received feedback.

This refinement process continues until:

- Customer requirements are completely satisfied.
- Missing features are added.
- Unnecessary features are removed.
- User Interface improvements are completed.
- Functional issues are resolved.

The Prototype Model follows this iterative cycle until customer approval is obtained.

---

## Phase 6: Product Development

### Description

After the customer approves the final prototype, developers begin developing the actual software application.

Unlike the prototype, the final product includes:

- Complete Business Logic
- Database Integration
- Security Features
- Performance Optimization
- Error Handling
- Complete Functionality

The approved prototype acts as the blueprint for software development.

---

## Phase 7: Testing

### Description

After development is completed, the Quality Assurance (QA) team tests the complete application.

Testing activities include:

- Functional Testing
- Integration Testing
- System Testing
- Acceptance Testing
- Regression Testing

Any identified defects are reported to developers for correction before deployment.

---

## Phase 8: Deployment

### Description

Once testing is completed successfully, the software is deployed to the customer's production environment.

The deployment team ensures:

- Successful installation
- Configuration
- User accessibility
- Production readiness

The software is then released for end users.

---

## Phase 9: Maintenance

### Description

Maintenance begins after the software is deployed.

The maintenance team performs:

- Bug Fixing
- Performance Improvements
- Feature Enhancements
- Security Updates
- Software Upgrades

Maintenance ensures the software continues to operate efficiently throughout its lifecycle.

## Types of Prototype

During software development, different types of prototypes are created depending on the project requirements.

The two commonly used types are:

1. **Static Prototype**
2. **Dynamic Prototype**

### 1. Static Prototype

A **Static Prototype** is a non-functional representation of the software application. It only demonstrates the appearance and layout of the system without implementing any actual functionality.

A static prototype is generally created using:

- Wireframes
- Mockups
- Screen Designs
- Flow Diagrams

The user can view the application screens, but no operations can be performed.

#### Characteristics

- **Displays only the User Interface (UI).**
- **Does not contain business logic.**
- **Cannot interact with the database.**
- **Used for requirement validation.**
- **Easy and inexpensive to develop.**

#### Example

A designer creates the login page, home page, and dashboard screens using design software such as **Figma** or **Adobe XD**.

The customer can review the appearance but cannot log in or perform any operations.

This is called a **Static Prototype**.

---

### 2. Dynamic Prototype

A **Dynamic Prototype** is a working model of the software that allows users to interact with the application.

Unlike a static prototype, a dynamic prototype implements some of the application's functionality.

Customers can execute certain operations and provide feedback based on the application's behavior.

#### Characteristics

- **Contains basic functionality.**
- **Allows user interaction.**
- **Implements partial business logic.**
- **Can perform limited operations.**
- **Provides better understanding of the final system.**

#### Example

A banking application prototype allows users to:

- Login
- View Account Balance
- Deposit Money

However, advanced features such as loan processing or fund transfers may not yet be implemented.

This is an example of a **Dynamic Prototype**.

---

## Types of Testing Performed in the Prototype Model

The Prototype Model mainly involves two types of testing.

1. **Prototype Testing**
2. **Actual Testing**

### 1. Prototype Testing

Prototype Testing is performed on the prototype before the actual software is developed.

The objective is to verify whether the prototype satisfies the customer's expectations.

During Prototype Testing:

- User Interface is verified.
- Navigation is checked.
- Workflow is validated.
- Customer feedback is collected.
- Missing requirements are identified.

Prototype Testing helps reduce development risks by identifying requirement-related issues at an early stage.

---

### 2. Actual Testing

After the customer approves the prototype, the complete software application is developed.

The developed application undergoes comprehensive software testing before deployment.

Actual Testing includes:

- Functional Testing
- Integration Testing
- System Testing
- Acceptance Testing
- Regression Testing
- Performance Testing
- Security Testing

The purpose is to ensure that the final software satisfies all business and technical requirements.

---

## Advantages of the Prototype Model

- **Users actively participate throughout software development.**
- **Customer feedback is collected at every iteration.**
- **Missing requirements are identified at an early stage.**
- **Requirement misunderstandings are minimized.**
- **Improves communication between developers and customers.**
- **Customer satisfaction is significantly higher.**
- **Reduces the risk of software failure.**
- **Changes can be incorporated before actual development begins.**
- **Very useful when project requirements are unclear.**
- **Improves overall software quality.**

---

## Disadvantages of the Prototype Model

- **Developing prototypes requires additional time.**
- **Development cost increases because multiple prototypes may be created.**
- **Frequent customer changes may delay the project.**
- **Poor documentation due to continuously changing requirements.**
- **Customers may expect the prototype to become the final product immediately.**
- **Developers may create low-quality solutions to quickly satisfy customers.**
- **Managing repeated iterations can become difficult.**
- **Not suitable for projects with well-defined requirements.**

---

## Real-Time Example

Suppose a company wants to develop an **Online Food Delivery Application**.

Initially, the customer is unsure about the application's design and required features.

The development team first creates a prototype containing:

- Login Screen
- Home Page
- Restaurant List
- Cart Page

The customer reviews the prototype and requests:

- Dark Mode
- Live Order Tracking
- Coupon System
- Digital Wallet

The prototype is updated several times until the customer is satisfied.

Only after approval does the development team build the complete software application.

This is a practical example of the **Prototype Model**.

---

## When to Use the Prototype Model

The Prototype Model is most suitable when:

- **Requirements are not clearly defined.**
- **Customer interaction is very important.**
- **Frequent requirement changes are expected.**
- **User Interface design is critical.**
- **The project is innovative or exploratory.**
- **Early customer feedback is required.**

---

## Key Points

- **The Prototype Model follows an iterative development approach.**
- **A prototype is created before developing the final software.**
- **Customer feedback plays an important role.**
- **The prototype is refined until customer approval is obtained.**
- **Static Prototypes display only the interface.**
- **Dynamic Prototypes provide working functionality.**
- **Prototype Testing is performed before actual software development.**
- **Actual Testing is performed after the final application is developed.**
- **The Prototype Model is ideal for projects with unclear or changing requirements.**

---

## Summary

The **Prototype Model** is an iterative Software Development Life Cycle (SDLC) model that focuses on understanding customer requirements by developing a working prototype before building the final software. Through continuous customer feedback and repeated refinement, the development team produces software that closely matches user expectations. The model minimizes requirement-related risks, improves customer satisfaction, and is particularly suitable for projects where requirements are uncertain or evolve over time.
