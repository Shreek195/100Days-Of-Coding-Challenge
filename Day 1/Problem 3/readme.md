# Magnets

This repository contains a solution to the Codeforces problem **"Magnets"** (Problem 344A). You can find the problem statement [here](https://codeforces.com/contest/344/problem/A).

## Intuition

The problem requires counting the number of contiguous groups of magnets with the same orientation. Each change in orientation signifies the start of a new group.

## Approach

1. **Read Input**: Parse the number of magnets and their orientations.
2. **Initialize Variables**: Use a variable to keep track of the current orientation and the number of groups.
3. **Process Each Magnet**:
   - Compare the current magnet's orientation with the previous one.
   - Increment the group count if the orientation changes.
4. **Output the Result**: Print the total number of groups.

## Complexity

- **Time Complexity**: O(n), where `n` is the number of magnets. Each magnet is processed exactly once.
- **Space Complexity**: O(1). The space used is constant, not depending on the input size.
