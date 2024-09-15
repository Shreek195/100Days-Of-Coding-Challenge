# Soldier and Bananas

This repository contains a solution to the Codeforces problem **"Soldier and Bananas"** (Problem A). You can find the problem statement [here](https://codeforces.com/problemset/problem/546/A).

## Intuition

The task is to determine how much money the soldier needs to borrow in order to buy a given number of bananas. The cost of each subsequent banana increases by a factor of the number of the banana, i.e., the i-th banana costs `i * k` dollars. The total cost is the sum of the arithmetic progression of the banana prices, and the soldier needs to borrow the difference between the total cost and the money he has, if the total cost exceeds his available money.

## Approach

1. **Input**:
   - Read the values `k` (cost of the first banana), `n` (initial amount of money the soldier has), and `w` (number of bananas the soldier wants).

2. **Calculate Total Cost**:
   - The cost of the bananas follows an arithmetic progression: the first banana costs `k`, the second costs `2k`, and so on up to `wk` for the w-th banana.
   - The total cost can be computed using the formula for the sum of the first `w` terms of an arithmetic progression: 
     \[
     \text{total cost} = k \times \left(\frac{w \times (w + 1)}{2}\right)
     \]

3. **Calculate Borrowing Amount**:
   - If the total cost exceeds the money the soldier has, the difference is the amount he needs to borrow. If he has enough money, no borrowing is required, so output `0`.

4. **Output Result**:
   - Print the amount the soldier needs to borrow. If no borrowing is necessary, print `0`.

## Complexity

- **Time Complexity**: O(1), as the total cost calculation and comparison are done in constant time.
- **Space Complexity**: O(1), since we only store a few variables and no additional data structures are needed.
