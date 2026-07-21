# Longest Valid Parentheses

## Problem Statement
Given a string containing just the characters '(' and ')', find the length of the longest valid (well-formed) parentheses substring.

## Approach (Stack)
- Use a stack to store indexes.
- Initialize stack with -1 (base index).
- Traverse string:
  - If '(' → push index
  - If ')' → pop
    - If stack becomes empty → push current index
    - Else → calculate length = i - stack.peek()
- Track maximum length.

## Time & Space Complexity
- Time Complexity: O(n)
- Space Complexity: O(n)
