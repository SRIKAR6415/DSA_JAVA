
# LeetCode 2 - Add Two Numbers

## Concept
Singly Linked List

## Approach
- Traverse both linked lists simultaneously.
- Add corresponding digits and previous carry.
- Store sum % 10 in a new node.
- Update carry using sum / 10.
- Continue until both lists and carry are empty.

## Example
Input:
l1 = [2,4,3]
l2 = [5,6,4]

Output:
[7,0,8]

## Complexity
Time Complexity: O(max(m,n))
Auxiliary Space: O(1), excluding output list.

## Important Concepts
- ListNode
- Dummy Node
- Current Pointer
- Carry
- Linked List Traversal
