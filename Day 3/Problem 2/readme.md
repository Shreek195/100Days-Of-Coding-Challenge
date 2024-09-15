# Elephant

This repository contains a solution to the Codeforces problem **"Elephant"** (Problem A). You can find the problem statement [here](https://codeforces.com/problemset/problem/617/A).

## Intuition

The task is to find the minimum number of steps the elephant needs to take to reach his friend's house located at point `x` on a coordinate line. The elephant can move by 1, 2, 3, 4, or 5 units in one step. The minimum number of steps can be determined by always trying to take the largest possible step of size 5, and calculating how many such steps are needed.

## Approach

1. **Input**: 
   - Read the integer `x`, which is the location of the friend's house.

2. **Optimal Step Calculation**:
   - The elephant should take as many steps of length 5 as possible to minimize the total number of steps.
   - The minimum number of steps can be calculated by dividing `x` by 5 and taking the ceiling of the result. This can be efficiently done using integer arithmetic by calculating `(x + 4) / 5`, which ensures any remainder is rounded up.

3. **Output**:
   - Print the result, which is the minimum number of steps needed to reach point `x`.

## Complexity

- **Time Complexity**: O(1), as the calculation of the number of steps is done in constant time.
- **Space Complexity**: O(1), since only a fixed amount of space is required to store the input and perform the calculation.
