
# LeetCode 7 - Reverse Integer

## Concept
Mathematics / Number Reversal

## Problem
Reverse the digits of a given 32-bit signed integer.
If the reversed integer exceeds the 32-bit signed integer range, return 0.

## Approach
1. Initialize reversed = 0.
2. Extract the last digit using x % 10.
3. Check whether adding the digit will cause integer overflow.
4. Build the reversed number using reversed * 10 + digit.
5. Remove the last digit using x / 10.
6. Repeat until x becomes 0.
7. Return the reversed number.

## Example 1
Input: 123
Output: 321

## Example 2
Input: -123
Output: -321

## Example 3
Input: 120
Output: 21

## Example 4
Input: 1534236469
Output: 0

## Important Concepts
- Modulus operator (%)
- Integer division (/)
- While loop
- Integer overflow
- Integer.MAX_VALUE
- Integer.MIN_VALUE

## Overflow Condition
Java int range:
- Maximum: 2147483647
- Minimum: -2147483648

Before calculating reversed * 10 + digit:
- Check positive overflow using MAX_VALUE / 10 and digit > 7.
- Check negative overflow using MIN_VALUE / 10 and digit < -8.

If overflow occurs, return 0.

## Complexity
Time Complexity: O(log10(|x|))
Space Complexity: O(1)

## Key Learning
Digit reversal is similar to Palindrome Number, but this problem requires additional handling for 32-bit integer overflow.
