# Bug Fixing Using Cursor AI

## Project Overview
This project demonstrates how AI-assisted debugging can help identify and fix errors in a Python program. Cursor AI was used to analyze the code, explain the bugs, and suggest corrections. Unit testing was performed using Python's `unittest` module in Google Colab.

## Objective
- Identify logical errors in a Python program.
- Use Cursor AI to understand and fix the bugs.
- Verify the corrections using unit tests.

## Project Files
- `student_utils.py` – Contains the corrected Python functions for calculating averages, checking pass marks, and assigning grades.
- `test_student_utils.py` – Contains unit tests for verifying the program's behavior.

## Bugs Identified and Fixed

### 1. Incorrect Average Calculation
**Problem:** The program divided the total marks by `len(marks) - 1`.

**Fix:** Changed the divisor to `len(marks)` so the average is calculated correctly.

### 2. Incorrect Passing Condition
**Problem:** The program used `mark > PASS_MARK`, so a student scoring exactly 40 was incorrectly considered to have failed.

**Fix:** Changed the condition to `mark >= PASS_MARK`.

### 3. Incorrect Grade Checking Order
**Problem:** The condition `average >= 60` was checked before `average >= 90`, making the Distinction condition unreachable.

**Fix:** Checked the highest grade condition first, followed by the lower grade conditions.

## Role of Cursor AI
Cursor AI was used to analyze the Python code, identify logical errors, explain why they were incorrect, and suggest fixes. The suggested changes were reviewed and applied to the program.

## Testing and Results
The program was tested using Python's `unittest` module in Google Colab.

- Initial testing identified errors in the original program.
- After applying the fixes, all 9 unit tests passed.
- The final output was `OK`.

## Technologies Used
- Python
- Cursor AI
- Google Colab
- Python `unittest` module

## Conclusion
This project demonstrates how Cursor AI can assist with debugging and how unit testing can verify that corrected code behaves as expected.
