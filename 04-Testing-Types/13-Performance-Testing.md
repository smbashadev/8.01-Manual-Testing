# Performance Testing

## Introduction

Modern software applications are expected to perform efficiently even when accessed by thousands or millions of users simultaneously. If an application becomes slow, unresponsive, or crashes under heavy traffic, it negatively affects the user experience and business reputation.

**Performance Testing** evaluates the responsiveness, stability, scalability, and reliability of a software application under different workload conditions.

It helps identify performance bottlenecks before the software is deployed into production.

---

## Definition

**Performance Testing** is a **Non-Functional Testing** technique performed to determine the **responsiveness**, **speed**, **stability**, and **scalability** of a software application under different workloads.

The primary objective of Performance Testing is to ensure that the software performs efficiently under expected and unexpected user loads.

---

## Objectives of Performance Testing

Performance Testing is performed to:

- **Measure application response time.**
- **Evaluate system stability.**
- **Determine maximum user capacity.**
- **Identify performance bottlenecks.**
- **Ensure application scalability.**
- **Improve user experience.**

---

## Types of Performance Testing

Performance Testing is mainly classified into four types:

1. **Load Testing**
2. **Stress Testing**
3. **Soak Testing**
4. **Spike Testing**

---

# 1. Load Testing

## Definition

**Load Testing** is the simplest form of Performance Testing performed to understand the behavior of the software under **expected user loads**.

The objective is to verify that the application performs efficiently when the expected number of users access the system simultaneously.

---

## Example

Suppose a Facebook server is expected to handle **50,000 users**.

The application is tested using gradually increasing user loads.

```text
Facebook Server

1,000 Users
      │
      ▼
2,000 Users
      │
      ▼
20,000 Users
      │
      ▼
30,000 Users
      │
      ▼
50,000 Users
```

The Test Engineer measures:

- Response Time
- CPU Usage
- Memory Usage
- Server Stability

---

## Advantages of Load Testing

- **Measures application performance under expected load.**
- **Identifies response time issues.**
- **Improves application scalability.**
- **Ensures stable user experience.**

---

# 2. Stress Testing

## Definition

**Stress Testing** is a type of Performance Testing performed to determine the **upper limit capacity** of the software and to observe how the application behaves when the load exceeds the expected maximum.

The objective is to determine the application's breaking point and recovery capability.

---

## Example

Expected Capacity:

**50,000 Users**

Actual Test Load:

```text
Facebook Server

50,001 Users
      │
      ▼
50,002 Users
      │
      ▼
50,003 Users
```

The Test Engineer verifies:

- Does the application crash?
- Does it recover automatically?
- Are error messages displayed correctly?

---

## Advantages of Stress Testing

- **Determines maximum system capacity.**
- **Identifies breaking point.**
- **Improves application reliability.**
- **Helps prevent production failures.**

---

# 3. Soak Testing

## Definition

**Soak Testing** is a type of Performance Testing performed to verify the **endurance** of a software application.

It evaluates whether the application remains stable while handling a continuous workload for a long period.

---

## Example

The Facebook server continuously handles:

```text
Facebook Server

2,000 Users
      │
      ▼
2,000 Users
      │
      ▼
2,000 Users
      │
      ▼
2,000 Users
      │
      ▼
2,000 Users
```

The workload remains constant for several hours or even days.

The Test Engineer monitors:

- Memory Usage
- CPU Utilization
- Resource Leaks
- System Stability

---

## Advantages of Soak Testing

- **Detects memory leaks.**
- **Measures long-term stability.**
- **Improves application endurance.**
- **Ensures reliable continuous operation.**

---

# 4. Spike Testing

## Definition

**Spike Testing** is a type of Performance Testing performed by suddenly increasing or decreasing the number of users and measuring the application's performance.

The objective is to verify whether the application can handle sudden traffic spikes without failure.

---

## Example

```text
Facebook Server

10,000 Users
      │
      ▼
20,000 Users
      │
      ▼
10,000 Users
      │
      ▼
30,000 Users
      │
      ▼
50,000 Users
```

The Test Engineer verifies:

- Response Time
- Server Recovery
- Error Handling
- Stability

---

## Advantages of Spike Testing

- **Validates sudden traffic handling.**
- **Improves scalability.**
- **Identifies performance bottlenecks.**
- **Ensures server stability during traffic spikes.**

---

## Comparison Table

| **Testing Type** | **Purpose** | **Workload Pattern** |
|------------------|-------------|----------------------|
| **Load Testing** | Verify expected workload performance. | Gradually increasing workload. |
| **Stress Testing** | Determine maximum capacity. | Load beyond expected limits. |
| **Soak Testing** | Verify endurance over time. | Constant workload for a long duration. |
| **Spike Testing** | Verify sudden traffic changes. | Sudden increase and decrease in workload. |

---

## Real-Time Examples

### Load Testing

An **Online Banking Application** is tested with **10,000 simultaneous users** to verify that Login, Fund Transfer, and Balance Enquiry work efficiently.

---

### Stress Testing

An **E-commerce Application** designed for **50,000 users** is tested with **75,000 users** to determine its maximum capacity.

---

### Soak Testing

A **Video Streaming Platform** is continuously tested for **72 hours** to verify that the server remains stable without memory leaks.

---

### Spike Testing

An **Online Ticket Booking Application** experiences a sudden increase in traffic when movie tickets or cricket match tickets become available.

Spike Testing verifies whether the application can handle these sudden user surges.

---

## Frequently Asked Interview Questions

### 1. What is Performance Testing?

Performance Testing is a Non-Functional Testing technique used to measure the responsiveness, stability, scalability, and speed of a software application under different workloads.

---

### 2. Is Performance Testing Functional or Non-Functional?

**Non-Functional Testing.**

---

### 3. Name the four types of Performance Testing.

- Load Testing
- Stress Testing
- Soak Testing
- Spike Testing

---

### 4. Which Performance Testing determines the maximum capacity of a software application?

**Stress Testing.**

---

### 5. Which Performance Testing verifies long-term stability?

**Soak Testing.**

---

### 6. Which Performance Testing verifies sudden traffic changes?

**Spike Testing.**

---

## Key Points

- **Performance Testing is a Non-Functional Testing technique.**
- **Measures speed, stability, responsiveness, and scalability.**
- **Load Testing verifies expected workload.**
- **Stress Testing determines maximum capacity.**
- **Soak Testing evaluates endurance over time.**
- **Spike Testing validates sudden workload changes.**
- **Performance Testing helps deliver reliable and scalable software.**

---

## Summary

**Performance Testing** is a Non-Functional Testing technique used to evaluate the responsiveness, stability, scalability, and reliability of software applications under different workload conditions. It includes **Load Testing**, **Stress Testing**, **Soak Testing**, and **Spike Testing**, each focusing on a specific aspect of application performance. Performance Testing ensures that software remains stable, responsive, and reliable under both normal and extreme usage conditions, thereby improving user satisfaction and reducing production failures.
