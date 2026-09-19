## Question 41

### What is Smoke Testing?

Smoke Testing is a preliminary level of testing performed on a new software build to verify that the critical functionalities work correctly before detailed testing begins.

It is also known as **Build Verification Testing (BVT).**

### Objectives

- Verify build stability
- Ensure critical features work
- Decide whether the build is suitable for further testing

### Example

After installing a new build of an e-commerce application, a tester verifies:

- Application launches successfully
- User can log in
- Homepage loads correctly
- Database connection works

If any of these fail, the build is rejected.

---

## Question 42

### What is Sanity Testing?

Sanity Testing is a narrow and focused testing process performed after bug fixes or minor changes to verify that the specific functionality works correctly.

### Objectives

- Validate recent changes
- Ensure bug fixes work
- Avoid unnecessary regression testing

### Example

If the Login module is fixed, the tester only tests the Login functionality instead of testing the entire application.

---

## Question 43

### What is the Difference Between Smoke Testing and Sanity Testing?

| Smoke Testing | Sanity Testing |
|---------------|----------------|
| Performed on a new build | Performed after bug fixes |
| Covers major functionalities | Covers specific functionality |
| Broad testing | Narrow testing |
| Determines build stability | Determines correctness of fixes |
| Executed before detailed testing | Executed before regression testing |

---

## Question 44

### What is Regression Testing?

Regression Testing is the process of re-testing previously working functionalities after changes, enhancements, or bug fixes to ensure that existing features continue to work correctly.

### Objectives

- Detect side effects
- Maintain software stability
- Verify existing functionality

### Example

A developer fixes the Payment module.

The tester verifies:

- Login
- Product Search
- Cart
- Payment
- Order History

to ensure nothing else is affected.

---

## Question 45

### What is Retesting?

Retesting is the process of executing failed test cases again after developers fix the reported defects.

### Objectives

- Verify bug fixes
- Confirm defect resolution

### Example

Bug:
User cannot log in using valid credentials.

After the developer fixes the issue, the tester executes the same Login test case again.

---

## Question 46

### What is the Difference Between Regression Testing and Retesting?

| Regression Testing | Retesting |
|--------------------|-----------|
| Checks unaffected areas | Checks fixed defect |
| Ensures existing functionality works | Confirms bug is fixed |
| Wide scope | Narrow scope |
| Usually automated | Usually manual |

---

## Question 47

### What is Functional Testing?

Functional Testing verifies whether every feature of the software behaves according to the specified functional requirements.

### Examples

- Login
- Registration
- Search
- Payment
- Logout

Functional testing focuses on **what the application does.**

---

## Question 48

### What is Non-Functional Testing?

Non-Functional Testing verifies aspects other than functionality, such as performance, usability, security, reliability, scalability, and compatibility.

### Examples

- Performance Testing
- Load Testing
- Stress Testing
- Security Testing
- Usability Testing
- Compatibility Testing

---

## Question 49

### What is Black Box Testing?

Black Box Testing is a testing technique in which the tester verifies application functionality without knowing the internal source code.

The tester only provides inputs and verifies outputs.

### Characteristics

- No programming knowledge required
- Focuses on user requirements
- Most common in Manual Testing

---

## Question 50

### What is White Box Testing?

White Box Testing is a testing technique in which the tester has knowledge of the application's internal code, logic, and structure.

It mainly focuses on:

- Code coverage
- Decision coverage
- Branch coverage
- Statement coverage

Usually performed by developers.

---

## Question 51

### What is Gray Box Testing?

Gray Box Testing combines Black Box and White Box Testing.

The tester has partial knowledge of the application's internal structure while testing externally.

### Advantages

- Better test coverage
- Efficient defect detection
- Improved integration testing

---

## Question 52

### What is Static Testing?

Static Testing verifies software artifacts without executing the application.

### Examples

- Requirement Review
- Design Review
- Code Review
- Walkthrough
- Inspection

### Benefits

- Detects defects early
- Saves cost
- Improves software quality

---

## Question 53

### What is Dynamic Testing?

Dynamic Testing verifies software by executing the application.

### Examples

- Functional Testing
- Regression Testing
- Integration Testing
- System Testing

Dynamic testing validates the actual behavior of the application.

---

## Question 54

### What is Ad-hoc Testing?

Ad-hoc Testing is an informal testing technique performed without predefined test cases or documentation.

The tester randomly explores the application to identify defects.

### Advantages

- Quick
- Flexible
- Finds unexpected bugs

---

## Question 55

### What is Exploratory Testing?

Exploratory Testing is a testing approach where learning, test design, and execution occur simultaneously.

The tester explores the application while continuously designing new test cases.

### Benefits

- Discovers hidden defects
- Requires experienced testers
- Improves product quality

---

## Question 56

### What is Monkey Testing?

Monkey Testing involves randomly providing unexpected inputs without following predefined test cases.

The objective is to determine whether the application crashes under unexpected conditions.

### Example

Randomly clicking buttons, entering invalid characters, or rapidly switching screens.

---

## Question 57

### What is Gorilla Testing?

Gorilla Testing focuses on repeatedly testing a single module until it becomes highly stable.

### Example

Testing the Login module hundreds of times using different combinations of:

- Valid credentials
- Invalid credentials
- Empty fields
- Boundary values

---

## Question 58

### What is Positive Testing?

Positive Testing verifies that the application behaves correctly when valid input data is provided.

### Example

Username: admin

Password: Admin@123

Expected Result:

Login Successful.

---

## Question 59

### What is Negative Testing?

Negative Testing verifies that the application handles invalid or unexpected input correctly.

### Example

Username: admin

Password: ######

Expected Result:

Invalid Username or Password.

---

## Question 60

### What is the Difference Between Positive Testing and Negative Testing?

| Positive Testing | Negative Testing |
|------------------|------------------|
| Uses valid data | Uses invalid data |
| Checks expected behavior | Checks error handling |
| Verifies success scenarios | Verifies failure scenarios |
| Ensures correct functionality | Ensures application robustness |

---

# End of Part 3 (Questions 41–60)

## Part 4 (Questions 61–80) will cover

- Integration Testing
- Big Bang Integration Testing
- Top-Down Integration Testing
- Bottom-Up Integration Testing
- Hybrid Integration Testing
- System Testing
- User Acceptance Testing (UAT)
- Alpha Testing
- Beta Testing
- Installation Testing
- Compatibility Testing
- Browser Compatibility Testing
- Cross-Platform Testing
- Usability Testing
- Accessibility Testing
- Security Testing
- Performance Testing
- Load Testing
- Stress Testing
- Volume Testing
