# Security Testing

## Introduction

Security is one of the most critical aspects of any software application. A secure application protects sensitive information from unauthorized access, data theft, and malicious attacks.

**Security Testing** verifies that only authorized users can access protected resources and that confidential information remains secure. It helps identify security vulnerabilities before the software is released into production.

Security Testing is considered one of the important **Non-Functional Testing** techniques.

---

## Definition

**Security Testing** is a type of testing in which a Test Engineer verifies the security of a software application by concentrating on the following aspects:

1. **Authentication Testing**
2. **Direct URL Testing**
3. **Firewall Leakage Testing**

The primary objective of Security Testing is to ensure that unauthorized users cannot access protected resources or confidential information.

---

## Objectives of Security Testing

Security Testing is performed to:

- **Protect sensitive information.**
- **Prevent unauthorized access.**
- **Verify user authentication.**
- **Protect confidential business data.**
- **Identify security vulnerabilities.**
- **Improve application reliability.**

---

## Security Components

```text
                    Gmail Application

                     Login Page
                          │
                          ▼
                    Authentication
                          │
            ┌─────────────┴─────────────┐
            │                           │
      Valid Credentials          Invalid Credentials
            │                           │
            ▼                           ▼
      Authorized Pages          Unauthorized Access
            │
    ┌───────┼────────┬──────────┐
    ▼       ▼        ▼          ▼
 Inbox   Compose   Draft   Sent Mail
                           │
                           ▼
                         Trash
```

---

# 1. Authentication Testing

## Definition

**Authentication Testing** is a type of Security Testing in which the Test Engineer verifies whether only authorized users can access the application by entering different combinations of **Username** and **Password**.

The objective is to ensure that only valid users are allowed to log into the system.

---

## Authentication Test Scenarios

The Test Engineer verifies:

- Valid Username + Valid Password
- Valid Username + Invalid Password
- Invalid Username + Valid Password
- Invalid Username + Invalid Password
- Empty Username
- Empty Password
- Empty Username and Password

---

## Example

Login Screen

```text
----------------------------

Username : ___________

Password : ___________

        [ Login ]

----------------------------
```

### Expected Result

- Valid credentials → Login Successful.
- Invalid credentials → Appropriate error message should be displayed.

---

# 2. Direct URL Testing

## Definition

**Direct URL Testing** is a type of Security Testing in which the Test Engineer copies the direct URL of an **Authorized Page** and pastes it into different browsers without logging into the application.

The objective is to verify whether unauthorized users can access protected pages directly.

---

## Example

Suppose the following page is available only after Login.

```text
https://gmail.com/inbox
```

The Test Engineer:

- Opens a new browser.
- Does not log in.
- Pastes the above URL directly.

### Expected Result

The application should redirect the user to the **Login Page**.

If the Inbox page opens directly, it is considered a **Security Defect**.

---

## Direct URL Workflow

```text
User
 │
 ▼
Copy Authorized URL
 │
 ▼
Open New Browser
 │
 ▼
Paste URL
 │
 ▼
Application
 │
 ├───────────────┐
 │               │
 ▼               ▼
Redirect      Opens
to Login      Protected Page
 │               │
Secure      Security Issue
```

---

# 3. Firewall Leakage Testing

## Definition

**Firewall Leakage Testing** is a type of Security Testing in which the Test Engineer logs into the application as one level of user and attempts to access resources or data that belong to another authorization level.

If unauthorized data is successfully accessed, it indicates a **Firewall Leakage** or **Access Control Vulnerability**.

---

## Diagrammatic Representation

```text
                   Internet User
                         │
                         ▼
                 Login as Employee
                         │
                         ▼
                  Application Firewall
                ┌─────────────────────┐
                │ Authentication Done │
                └──────────┬──────────┘
                           │
                           ▼
                 Employee Dashboard
                           │
                           │
          Attempts to Access Admin Data
                           │
                 ┌─────────┴─────────┐
                 │                   │
                 ▼                   ▼
          Access Denied        Admin Data Visible
                 │                   │
            Application         Firewall Leakage
             is Secure        Security Vulnerability
```

---

## Example

Suppose an application contains two user roles.

### Employee

Can access:

- Profile
- Attendance
- Salary Slip

---

### Administrator

Can access:

- Employee Records
- Payroll
- Reports
- User Management

If an **Employee** logs in and successfully accesses the **Payroll Module**, then the application contains a **Firewall Leakage**.

---

## Advantages of Security Testing

- **Protects confidential information.**
- **Prevents unauthorized access.**
- **Improves software reliability.**
- **Protects customer data.**
- **Reduces security risks.**
- **Improves customer trust.**

---

## Disadvantages of Security Testing

- **Requires experienced security testers.**
- **Time-consuming.**
- **Requires specialized testing tools.**
- **Cannot guarantee complete security.**

---

## Real-Time Examples

### Authentication Testing

A user attempts to log into Gmail using different Username and Password combinations.

The Login page should allow only valid users.

---

### Direct URL Testing

A user directly enters:

```text
https://mail.company.com/inbox
```

without logging in.

The application should redirect the user to the Login page.

---

### Firewall Leakage Testing

An employee logs into the HR Management System and manually changes the URL to access the Admin Dashboard.

If the Admin Dashboard opens successfully, it indicates a Firewall Leakage vulnerability.

---

## Comparison Table

| **Testing Type** | **Purpose** |
|------------------|-------------|
| **Authentication Testing** | Verifies valid Username and Password combinations. |
| **Direct URL Testing** | Verifies unauthorized access through direct URLs. |
| **Firewall Leakage Testing** | Verifies role-based access control and authorization. |

---

## Frequently Asked Interview Questions

### 1. What is Security Testing?

Security Testing is a Non-Functional Testing technique used to verify that only authorized users can access protected resources.

---

### 2. Name the three major types of Security Testing discussed in Manual Testing.

- Authentication Testing
- Direct URL Testing
- Firewall Leakage Testing

---

### 3. What is Authentication Testing?

Authentication Testing verifies whether only valid users can access the application using correct credentials.

---

### 4. What is Direct URL Testing?

Direct URL Testing verifies whether protected pages can be accessed without authentication.

---

### 5. What is Firewall Leakage Testing?

Firewall Leakage Testing verifies whether users can access resources beyond their authorization level.

---

## Key Points

- **Security Testing is a Non-Functional Testing technique.**
- **Authentication verifies user identity.**
- **Direct URL Testing verifies protected page access.**
- **Firewall Leakage Testing verifies authorization.**
- **Security Testing protects confidential business data.**
- **Prevents unauthorized access to applications.**

---

## Summary

**Security Testing** is a Non-Functional Testing technique used to protect software applications from unauthorized access and security vulnerabilities. It includes **Authentication Testing**, **Direct URL Testing**, and **Firewall Leakage Testing**, each verifying different aspects of application security. Security Testing helps ensure that only authorized users can access protected resources, confidential information remains secure, and role-based access control is enforced correctly, thereby improving the overall reliability and security of the application.
