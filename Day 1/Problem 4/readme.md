# Fair PlayOff

This repository contains a solution to the Codeforces problem **"Fair PlayOff"** (Problem 1535A). You can find the problem statement [here](https://codeforces.com/contest/1535/problem/A).

## Intuition

To determine if the tournament is fair, you need to verify if the two highest skill levels are among the finalists. Specifically:
1. Identify the top two skill levels.
2. Ensure these skills are present in the set of players who advance to the finals.

## Approach

1. **Read Input**: Parse the number of test cases.
2. **Process Each Test Case**:
   - Determine the skill levels of the four players.
   - Find the top two skills.
   - Check if these top two skills are in the winners' pool (the winners of the first and second rounds).
3. **Output the Result**: Print `"YES"` if the tournament is fair, otherwise print `"NO"`.

## Complexity

- **Time Complexity**: O(n), where `n` is the number of test cases. Each test case involves constant-time operations O(1).
- **Space Complexity**: O(1). The space used is constant and does not depend on the input size.
