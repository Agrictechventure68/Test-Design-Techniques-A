# Test-Design-Techniques-A
Exploring essential software testing strategies to determine expected outcome on product testing
🎯 Test Design Techniques Assignment

Test Design Techniques** assignment

In this assignment, I will explore essential software testing strategies including black-box and white-box testing, equivalence partitioning, boundary value analysis, decision tables, and state transition testing. Each technique is designed to boost software quality and improve defect detection.

1. Black-Box vs White-Box Testing

⚫ Black-Box Testing
Definition: Testing without knowing the internal structure of the application. Focuses on inputs and expected outputs.
  
 *Characteristics:
  - Based on specifications
  - No knowledge of code required
  - Functional and behavioral testing
  Example:  
  Testing a login page by entering valid and invalid credentials to verify correct error or success messages.

⚪ White-Box Testing
Definition: Testing based on the internal logic of the application. Testers must understand the code.

*Characteristics:
  - Requires programming skills
  - Covers code branches, loops, and conditions
  - Used mainly for unit testing
  Example:  
  Inspecting the `if-else` blocks in the authentication function to verify all logic paths are correctly tested.

---

2. Equivalence Partitioning (EP)
Definition: Dividing input data into valid and invalid partitions where the system is expected to behave similarly.

Purpose:
  - Reduces redundant test cases
  - Ensures good test coverage
  Example:  
  For an age input of 18–60:
  - Partition 1 (Invalid): `< 18`
  - Partition 2 (Valid): `18–60`
  - Partition 3 (Invalid): `> 60`  
    Test Values: `16`, `30`, `65`


3. Boundary Value Analysis (BVA)
Definition: Testing at the edges of input ranges where bugs often occur.

Purpose:
  - Captures off-by-one and edge-case errors
  Example:  
  For an age field `18–60`, test:
  - Lower boundary: `17`, `18`, `19`
  - Upper boundary: `59`, `60`, `61`

---

4. Decision Table Testing
Definition: Uses a tabular format to model complex business logic and combinations of inputs.

Purpose:
  - Helps visualize rule-based logic
  - Covers multiple input combinations
   
  Example:  
Loan Approval Conditions Table:

| Condition            | Rule 1 | Rule 2 | Rule 3 | Rule 4 |
|----------------------|--------|--------|--------|--------|
| Income > 50,000      | Yes    | Yes    | No     | No     |
| Credit Score > 700   | Yes    | No     | Yes    | No     |
| Loan Approved?       | Yes    | No     | No     | No     |



5. State Transition Testing
Definition: Focuses on system behavior when transitioning between different states.

Use Cases:
  - Best for applications with finite states
  - Ensures all transitions are handled correctly
   
  Example:  
ATM Machine State Transitions Table:

| Current State | Input         | Next State    | Output              |
|---------------|---------------|---------------|---------------------|
| Card Inserted | Enter PIN     | Authenticated | Show menu           |
| Authenticated | Withdraw Cash | Idle          | Dispense cash       |
| Authenticated | Eject Card    | Idle          | Thank you message   |


Folder structure:
test-design-techniques-assignment/
├── README.md ← Assignment documentation
├── state-transition.png ← (Optional: diagram image)
└── decision-table.png ← (Optional: visual for table)


9. Conclusion

Test design techniques help testers build efficient, targeted, and powerful test cases. Mastering these tools—black-box testing, equivalence partitioning, BVA, decision tables, and state transitions—ensures better software quality, fewer bugs, and happier users.

---

📌 *Created by [Bright Doro]*  
📅 *Submitted: [12/06/2025]
