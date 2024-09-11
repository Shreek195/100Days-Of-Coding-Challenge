# Tram Capacity Problem

This repository contains a solution to the Codeforces problem **"Tram Capacity Problem"** (Problem 116A). You can find the problem statement [here](https://codeforces.com/contest/116/problem/A).

## Intuition

To determine the minimum capacity required for the tram:
1. Track the number of passengers inside the tram as it moves from stop to stop.
2. Update the number of passengers after each stop based on the number exiting and entering.
3. Keep track of the maximum number of passengers inside the tram at any point.
4. The maximum observed number of passengers will be the minimum capacity required.

## Approach

1. **Read Input**: Parse the number of stops `n` and the number of passengers exiting and entering at each stop.
2. **Initialization**:
   - Start with zero passengers and initialize the capacity based on the number of passengers entering at the first stop.
3. **Process Each Stop**:
   - For each stop, adjust the number of passengers by subtracting those exiting and adding those entering.
   - Update the maximum capacity if the current number of passengers exceeds the previously recorded maximum.
4. **Output the Result**: Print the maximum capacity required to accommodate the passengers.

## Complexity

- **Time Complexity**: O(n), where `n` is the number of stops. Each stop is processed in constant time O(1).
- **Space Complexity**: O(1). The space used is constant and does not depend on the input size.
