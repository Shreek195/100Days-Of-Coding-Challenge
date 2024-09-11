# Codeforces Checking

This repository contains a solution to the Codeforces problem **"Checking"** (Problem 1791A). You can find the problem statement [here](https://codeforces.com/contest/1791/problem/A).

## Intuition

The task is to check if a given lowercase Latin letter appears in the string `"codeforces"`. Since `"codeforces"` is a fixed string with a small number of distinct characters, this problem can be solved efficiently by using a set for constant-time membership checks.

## Approach

1. **Preprocess the Characters**: Create a set containing the characters from the string `"codeforces"`. This allows for quick look-up operations.
2. **Check Each Character**: For each test case, check if the given character is present in the set of characters from `"codeforces"`.
3. **Output the Result**: Print `"YES"` if the character is in the set; otherwise, print `"NO"`.

## Complexity

- **Time Complexity**: O(n), where `n` is the number of test cases. Each test case involves a constant-time membership check in the set.
- **Space Complexity**: O(1). The space required to store the set of characters from `"codeforces"` is constant as the set size is fixed.
