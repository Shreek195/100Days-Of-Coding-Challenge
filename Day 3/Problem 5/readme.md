# In Search of an Easy Problem

This repository contains a solution to the Codeforces problem **"In Search of an Easy Problem"** (Problem A). You can find the problem statement [here](https://codeforces.com/problemset/problem/1030/A).

## Intuition

The problem requires checking whether a problem is considered easy or hard based on the opinions of `n` people. Each person provides a binary opinion: `0` means the problem is easy, and `1` means the problem is hard. If at least one person thinks the problem is hard, the entire problem is considered hard.

## Approach

1. **Input**:
   - The first line contains the integer `n`, which is the number of people asked.
   - The second line contains `n` integers, either `0` or `1`. A `0` indicates that the problem is easy, and a `1` indicates that the problem is hard.

2. **Check for Difficulty**:
   - Read the second line of input and remove all whitespace to create a single string of digits.
   - Convert the string to a numeric value and check if it's greater than `0`. If any person has said the problem is hard (i.e., if there is at least one `1`), the problem is hard, and we print "HARD". Otherwise, we print "EASY".

3. **Output Result**:
   - If the problem is considered hard by at least one person, print "HARD". Otherwise, print "EASY".

## Complexity

- **Time Complexity**: O(n), where `n` is the number of people. We process each input once, checking each response to see if the problem is considered hard.
- **Space Complexity**: O(n), as we store the input opinions in memory for analysis.
