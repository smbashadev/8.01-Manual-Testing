# Bug Life Cycle

## Introduction

During software testing, defects are identified by Test Engineers and reported to the Development Team for fixing. Every reported defect passes through several stages before it is finally closed.

The sequence of stages through which a defect passes from the time it is identified until it is permanently closed is known as the **Bug Life Cycle** or **Defect Life Cycle**.

Understanding the Bug Life Cycle helps ensure proper communication between the Testing Team and Development Team, improves defect management, and ensures that every reported defect is resolved effectively.

---

## Definition

**Bug Life Cycle** is the sequence of different states (stages) that a bug travels through from the time it is identified until it is finally closed.

It is also known as the **Defect Life Cycle**.

---

## Objectives of Bug Life Cycle

The Bug Life Cycle is followed to:

- **Track every reported defect.**
- **Monitor the progress of defect resolution.**
- **Improve communication between Testers and Developers.**
- **Ensure defects are fixed before software release.**
- **Maintain complete defect history.**
- **Improve software quality.**

---

## Bug Life Cycle Workflow

```text
                     Bug Identified
                           │
                           ▼
                         New
                           │
                           ▼
                        Assigned
                           │
                           ▼
                          Open
                           │
          ┌────────────────┴────────────────┐
          │                                 │
          ▼                                 ▼
        Fixed                           Rejected
          │                                 │
          ▼                                 ▼
         Test                          Closed
          │
     ┌────┴────┐
     │         │
     ▼         ▼
 Verified   Reopened
     │         │
     ▼         ▼
   Closed     Assigned
     │
     ▼
    Dead

          (Optional State)

        Deferred
             │
             ▼
   Fixed in Future Release
```

---

## Bug States

### 1. New

A bug is in the **New** state immediately after it is identified and reported by the Test Engineer.

At this stage:

- The defect is recorded.
- A unique Bug ID is assigned.
- The defect awaits assignment.

---

### 2. Assigned

The Project Manager, Test Lead, or QA Lead assigns the defect to the appropriate Developer.

The assigned Developer becomes responsible for analyzing and fixing the defect.

---

### 3. Open

The Developer opens the defect and starts analyzing it.

At this stage, the Developer:

- Reproduces the defect.
- Identifies the root cause.
- Begins fixing the issue.

---

### 4. Fixed

Once the Developer resolves the defect, its status is changed to **Fixed**.

The updated software build is then sent back to the Testing Team for verification.

---

### 5. Test

The Test Engineer performs **Retesting** to verify whether the reported defect has been fixed correctly.

Possible outcomes:

- Defect fixed successfully.
- Defect still exists.

---

### 6. Reopened

If the defect still exists after Retesting, the Test Engineer changes the status to **Reopened**.

The defect is reassigned to the Developer for further analysis and fixing.

---

### 7. Verified

If the Test Engineer confirms that the defect has been fixed successfully, the status changes to **Verified**.

The defect is now ready for closure.

---

### 8. Closed (Dead)

After successful verification, the defect is permanently closed.

The bug is considered **Dead**, meaning it no longer exists in the software.

---

### 9. Rejected

Sometimes the reported issue is **not actually a software defect**.

In such cases, the Developer rejects the defect.

Reasons may include:

- Expected behavior.
- Duplicate defect.
- Invalid defect.
- Incorrect testing.

---

### 10. Deferred

A defect may be marked as **Deferred** when the Development Team decides not to fix it in the current software version.

The defect will be fixed in a future release.

Reasons include:

- Low priority.
- Limited project time.
- Budget constraints.
- Feature scheduled for future enhancement.

---

## Complete Bug Life Cycle

```text
New
 │
 ▼
Assigned
 │
 ▼
Open
 │
 ├──────────────┐
 │              │
 ▼              ▼
Fixed       Rejected
 │              │
 ▼              ▼
Test         Closed
 │
 ├──────────────┐
 │              │
 ▼              ▼
Verified    Reopened
 │              │
 ▼              ▼
Closed      Assigned
 │
 ▼
Dead

(Optional)

Open
 │
 ▼
Deferred
 │
 ▼
Future Release
```

---

## Real-Time Example

Consider a **Gmail Login Application**.

Requirement:

The Password entered by the user should be displayed as **asterisks (*)**.

Actual Result:

The Password is displayed as plain text.

The Test Engineer reports the bug.

The defect passes through the following stages:

```text
New

↓

Assigned

↓

Open

↓

Fixed

↓

Test

↓

Verified

↓

Closed (Dead)
```

If the Password is still visible after Retesting:

```text
Test

↓

Reopened

↓

Assigned

↓

Open

↓

Fixed

↓

Verified

↓

Closed
```

---

## Advantages of Bug Life Cycle

- **Tracks every reported defect.**
- **Improves communication among project teams.**
- **Ensures defects are properly managed.**
- **Supports project monitoring.**
- **Improves software quality.**
- **Maintains complete defect history.**

---

## Difference Between Bug and Defect

| **Bug** | **Defect** |
|----------|------------|
| Informal term used by Developers and Testers. | Formal term used in software quality processes. |
| Represents an issue in the software. | Represents any deviation from expected behavior. |
| Usually discovered during testing. | May be discovered during development, testing, or production. |

---

## Frequently Asked Interview Questions

### 1. What is a Bug Life Cycle?

The Bug Life Cycle is the sequence of states that a software defect passes through from identification until closure.

---

### 2. What is another name for Bug Life Cycle?

**Defect Life Cycle.**

---

### 3. What happens in the Assigned state?

The defect is assigned to a Developer for analysis and fixing.

---

### 4. When is a bug marked as Reopened?

When the Test Engineer finds that the defect still exists after Retesting.

---

### 5. What is a Deferred defect?

A Deferred defect is postponed and planned to be fixed in a future software release.

---

### 6. What is the difference between Rejected and Deferred?

- **Rejected** means the reported issue is not considered a valid defect.
- **Deferred** means the defect is valid but will be fixed in a future release.

---

## Key Points

- **Bug Life Cycle is also called Defect Life Cycle.**
- **Every reported defect follows predefined states.**
- **Retesting is performed after the Developer fixes the defect.**
- **Reopened defects are reassigned to Developers.**
- **Deferred defects are fixed in future releases.**
- **Closed (Dead) indicates that the defect no longer exists.**

---

## Summary

The **Bug Life Cycle**, also known as the **Defect Life Cycle**, is a systematic process used to manage software defects from identification to closure. It consists of multiple stages including **New**, **Assigned**, **Open**, **Fixed**, **Test**, **Verified**, **Reopened**, **Rejected**, **Deferred**, and **Closed (Dead)**. Following a structured Bug Life Cycle helps organizations effectively track, manage, verify, and resolve defects, ultimately improving software quality and ensuring successful software delivery.
