# Word

This repository contains a solution to the Codeforces problem **"Word"** (Problem 59A). You can find the problem statement [here](https://codeforces.com/contest/59/problem/A).

## Intuition

To decide on the case conversion for the word, we need to count the number of uppercase and lowercase letters. Based on the counts, we will convert the word to the appropriate case:

- If uppercase letters are more than lowercase letters, the result should be in uppercase.
- Otherwise, the result should be in lowercase.

## Approach

1. **Read Input**: 
   - Read the word from the input.

2. **Count Uppercase and Lowercase Letters**:
   - Initialize counters for uppercase and lowercase letters.
   - Traverse through each character in the word:
     - Increment the uppercase counter if the character is uppercase.
     - Increment the lowercase counter if the character is lowercase.

3. **Determine and Output Result**:
   - Compare the counts of uppercase and lowercase letters.
   - Convert and print the word in uppercase if uppercase letters are more; otherwise, print it in lowercase.

Here's a summary of the code logic:

- **Input Reading**: Read the word using `BufferedReader`.
- **Counting Letters**: Loop through each character to count uppercase and lowercase letters.
- **Case Conversion**: Use Java's `toUpperCase()` and `toLowerCase()` methods to convert the word as needed based on the counts.

## Complexity

- **Time Complexity**: O(n), where n is the length of the word. This is because we traverse the word once to count the letters.
- **Space Complexity**: O(1). The space used is constant, as we only need a few variables to store the counts and the word itself.
