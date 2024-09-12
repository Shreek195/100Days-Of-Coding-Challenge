# 1929. Concatenation of Array

This repository contains a solution to the LeetCode problem **"Concatenation of Array"** (Problem 1929). You can find the problem statement [here](https://leetcode.com/problems/concatenation-of-array/description/).

## Intuition

To form the array `ans`, you need to create a new array that holds two copies of the original array `nums`. This can be achieved by iterating over the `nums` array and copying its elements into the appropriate positions in the `ans` array.

## Approach

1. **Initialize the Result Array**:
   - Create a new array `ans` with a length of `2n`.

2. **Populate the Result Array**:
   - Iterate through each element in the `nums` array.
   - Copy each element into the first half of the `ans` array.
   - Copy each element into the second half of the `ans` array by offsetting by the length of `nums`.

3. **Return the Result**:
   - Return the `ans` array as the result.

Here's a summary of the code logic:

- **Array Initialization**: Initialize an array `ans` with size `2 * nums.length`.
- **Array Population**: For each element in `nums`, assign it to both the current index and the index offset by `nums.length` in `ans`.

## Complexity

- **Time Complexity**: O(n), where `n` is the length of the `nums` array. The solution iterates through the `nums` array once, performing constant-time operations O(1) for each element.
- **Space Complexity**: O(n). The space used is proportional to the size of the result array, which is `2 * nums.length`.
