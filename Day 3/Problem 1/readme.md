# Odd One Out

This repository contains a solution to the Codeforces problem **"Odd One Out"** (Problem 1915A). You can find the problem statement [here](https://codeforces.com/contest/236/problem/A).

## Intuition

The task requires identifying the number that appears only once out of three given digits, where two are identical, and one is different. This can be achieved by simple comparisons of the three digits to determine which one is the odd one out.

## Approach

1. **Read Input**: 
   - First, read the number of test cases.
   - For each test case, read the three digits.

2. **Identify the Odd One**:
   - Compare the first two digits:
     - If they are the same, the third digit is the odd one.
     - Otherwise, compare the last two digits:
       - If they are the same, the first digit is the odd one.
       - Otherwise, the second digit is the odd one.

3. **Output Result**:
   - For each test case, print the digit that occurs exactly once.

## Complexity

- **Time Complexity**: O(n), where n is the number of test cases. Each test case requires constant time O(1) for comparisons.
- **Space Complexity**: O(1), as no additional space is needed apart from storing a few integer variables.
