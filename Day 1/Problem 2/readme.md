## Intuition

The problem requires checking if any of the three given integers can be expressed as the sum of the other two. Since the integers are small (from 0 to 20), a direct comparison approach is efficient.

## Approach

1. **Read Input**: Parse the number of test cases.
2. **Process Each Test Case**:
   - Read the three integers `a`, `b`, and `c`.
   - Check the following conditions:
     - If `a + b == c`
     - If `b + c == a`
     - If `c + a == b`
   - Print `"YES"` if any of these conditions hold true; otherwise, print `"NO"`.

## Complexity

- **Time Complexity**: O(n), where `n` is the number of test cases. Each test case involves a constant number of operations (3 checks).
- **Space Complexity**: O(1). The space required is constant as it only involves storing a few integers and performing basic operations.
