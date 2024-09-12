# Black Square

This repository contains a solution to the Codeforces problem **"Black Square"** (Problem 431A). You can find the problem statement [here](https://codeforces.com/contest/431/problem/A).

## Intuition

The task requires calculating the total calories Jury wastes based on the sequence of black squares appearing on different strips. Each strip has a defined calorie consumption rate, and the goal is to sum up the total calories based on the given sequence.

## Approach

1. **Read Input**: 
   - Read the calorie values for each strip.
   - Read the sequence string describing the appearance of black squares.

2. **Calculate Total Calories**:
   - Initialize a variable `sum` to store the total calories.
   - Iterate through each character in the sequence string.
   - Convert each character to its corresponding strip index and use it to find the associated calorie value.
   - Add this calorie value to `sum`.

3. **Output Result**:
   - Print the total calories computed.

The approach efficiently maps each character in the sequence to the respective calorie value and accumulates the total calories using simple indexing and summation.

## Complexity

- **Time Complexity**: O(n), where n is the length of the sequence string. This is because we iterate through the string once and perform constant-time operations O(1) for each character.
- **Space Complexity**: O(1). We use a fixed amount of extra space regardless of the input size (just a few integer variables).
