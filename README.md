# Lab Reflection: Git Version Control + Debugging (BuggyProgram)

## Student Name 
Chase Hilsinger.

## GitHub Repository URL
https://github.com/chasehils/Lab1-Github-JUnit

---

# Commit 1: Initial Commit

## What did you include in this commit?
- The intitial project structure of buggy Java program and JUnit test

## What was the purpose of this commit?
-To have a baseline version of the code

---

# Commit 2: Task 1 (getGrade)

## Which tests in Task1Test were failing before your fix?
-The threshold condition tests from grade boundaries

## What was the issue in the code?
-There was incorrect comparision operators using < or > instead of using <= or >=

## What change did you make to fix it?
-Updated the conditional boundary operators to match the grade scale requirements

## How did the tests help guide your fix?
-The JUnit failure messages pointed directly to the unexpected letter grade output for specific score inputs

---

# Commit 3: Task 2 (sumEvenNumbers)

## Which tests in Task2Test were failing before your fix?
-Tests checking the cumulative sum of even numbers over a given range or array

## What was the issue in the code?
-The loop incremenet or filtering logic skipped valid even numbers or improperly accumulated odd values

## What change did you make to fix it?
-adjusted the loop condition and modulus check (i % 2 == 0) to correct target only even numbers

## How did the tests help guide your fix?
- The test assertion errors showed the problem between the expected sum and the actua computed sum

---

# Commit 4: Task 3 (sumRange)

## Which tests in Task3Test were failing before your fix?
-Tests evaluating sumRange where final endpoint value was excluded from the total

## What was the issue in the code?
-An off by one error in the for loop condition (i < end instead of i <= end)

## What change did you make to fix it?
-changed the loop condition to less than or equal (<=)

## How did the tests help guide your fix?
-the tests failed with a total that was short  by the value of the end parameter

---

# Overall Reflection

## Which task was the easiest to fix? Why?
- Task 3 (sumRange) becuase an off by one loop boundary error is straightforward to spot and fix once the failing test output is found

## Which task was the most difficult? Why?
-Task 1, having to spot conditions to find incorrect operators can be difficult

## How did Git help you track your progress through the debugging process?
-By being able to to isolate bug fixes to track when each problem was solved

## Why is it important to make small, frequent commits when debugging code?
-It allows you to go back to previous code and find a bug if there is one

## What did you learn about using JUnit tests to guide debugging?
-testing can help to pinpoint where the errors are than manual print statements

---

# Commit 5: Final Reflection

## What did you complete or update before making this final commit?
-I filled out the README.md file documenting the debugging process

## Why is it useful to document your work after completing a programming task?
-It helps solves problems  and makes it clear for anyone to review the repository 