#  Boy or Girl

This repository contains a solution to the Codeforces problem **" Boy or Girl"** (Problem 236A). You can find the problem statement [here](https://codeforces.com/contest/236/problem/A).

## Intuition

To determine the gender based on the username, count the number of unique characters in the string. If this count is even, the user is female; if odd, the user is male. This is based on the observation that the presence of unique characters can be used to infer the gender according to the problem's criteria.

## Approach

1. **Read Input**: 
   - Read the username from the input.

2. **Count Distinct Characters**:
   - Initialize a counter to keep track of the number of unique characters.
   - Use a set or check manually if a character is distinct to count the unique characters.

3. **Determine Gender**:
   - Check if the count of unique characters is even or odd.
   - Print "CHAT WITH HER!" if the count is even.
   - Print "IGNORE HIM!" if the count is odd.

Here is a brief explanation of the code:

- **String Reading**: Read the username using `BufferedReader`.
- **Unique Character Counting**: Iterate through each character of the username. If it's not already in the results string, increment the counter and append the character to the results string.
- **Gender Determination**: Check if the count of unique characters (`ctr`) is even or odd and print the appropriate message.

## Complexity

- **Time Complexity**: O(n), where n is the length of the username. This is because we iterate through the string once and perform constant-time operations for each character.
- **Space Complexity**: O(n). The space is used to store the results string, which in the worst case could be as large as the length of the input string. However, this is manageable within the problem constraints.
