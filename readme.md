
# Longest Valid Parentheses

## Problem
Given a string containing only '(' and ')', find the length of the longest valid parentheses substring.

## Examples

**Example 1:**
```text
Input: s = "(()"
Output: 2
```

**Example 2:**
```text
Input: s = ")()())"
Output: 4
```

**Example 3:**
```text
Input: s = ""
Output: 0
```

## Approach

I used Dynamic Programming to solve this problem.

- Created a DP array where `dp[i]` stores the length of the longest valid parentheses substring ending at index `i`.
- If the current character is `)` and the previous character is `(`, we get a valid pair of length 2.
- If the previous character is also `)`, we check whether there is a matching `(` before the previous valid substring.
- Update the maximum length at each step.

## Complexity Analysis

- **Time Complexity:** O(n)
- **Space Complexity:** O(n)

## Language
C++
