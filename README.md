#  LeetCode 485: Max Consecutive Ones

##  Problem Statement
Given a binary array `nums`, return the maximum number of consecutive `1`'s in the array.



### Example
**Input:** `nums = [1,1,0,1,1,1]`  
**Output:** `3`  
**Explanation:** The first two digits or the last three digits are consecutive 1s. The maximum number of consecutive 1s is 3.

##  Intuition & Approach
The logic is to keep a running counter that tracks the current streak of ones and a "high score" variable to store the maximum streak found so far.

### Key Steps:
1. **Traverse** the array using an enhanced for-loop.
2. **Increment** a `count` variable every time we encounter a `1`.
3. **Compare** the `count` with `max` immediately to ensure we capture the highest streak.
4. **Reset** the `count` to `0` as soon as we hit a `0`.

Complexity Analysis 
Time Complexity: \(O(n)\) — We perform a single linear scan of the array.
Space Complexity: \(O(1)\) — We only use two integer variables (count and max), regardless of input size. 
