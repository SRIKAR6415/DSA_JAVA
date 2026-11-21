
# LeetCode 9 - Palindrome Number

## Concept
Number Reversal / Mathematics

## Approach
1. Store the original number in temp.
2. Extract the last digit using % 10.
3. Build the reversed number using reversed * 10 + digit.
4. Remove the last digit using / 10.
5. Compare the reversed number with the original.

## Example
Input: 121
Reversed: 121
Output: true

## Complexity
Time Complexity: O(log10(n))
Space Complexity: O(1)

## Important Concepts
- Modulus operator (%)
- Integer division (/)
- While loop
- Number reversal
