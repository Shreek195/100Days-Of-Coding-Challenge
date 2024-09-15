# Word Capitalization

This repository contains a solution to the Codeforces problem **"Word Capitalization"** (Problem A). You can find the problem statement [here](https://codeforces.com/problemset/problem/281/A).

## Intuition

The task is to capitalize the first letter of the given word while leaving the rest of the word unchanged. If the first letter is already capitalized, or if the word contains mixed-case letters, the rest of the word remains the same. This is essentially string manipulation, specifically modifying the case of the first character.

## Approach

1. **Input**:
   - Read a single word consisting of uppercase and lowercase English letters.

2. **Capitalize the First Letter**:
   - Extract the first character of the word and convert it to uppercase using the `toUpperCase()` method.
   - Concatenate the uppercase first character with the rest of the string (starting from the second character) which remains unchanged.

3. **Output the Result**:
   - Print the modified word.

## Complexity

- **Time Complexity**: O(n), where `n` is the length of the input word. This is because we process each character once, with constant time operations for extracting and converting the first character.
- **Space Complexity**: O(n), as we store a new string that is a modified version of the input word.
