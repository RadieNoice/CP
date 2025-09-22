# 34. Find First and Last Position of Element in Sorted Array

**Link:** https://leetcode.com/problems/find-first-and-last-position-of-element-in-sorted-array/submissions/1778554545/

Given an array of integers nums sorted in non-decreasing order, find the starting and ending position of a given target value. If target is not found in the array, return [-1, -1]. You must write an algorithm with O(log n) runtime complexity.


## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-5 suffer from incorrect binary search implementations for finding both start and end indices. Conditional logic within the loops is flawed, leading to incorrect index updates (`s`, `e`).  The `if(nums[m] < target)` is duplicated in the loops.

2. **Evolution**: There's no real improvement in the logic across attempts. The code remains fundamentally incorrect in its approach to finding the start and end indices.  The attempts repeatedly fail to correctly identify the boundary conditions for the target value in a sorted array using binary search.

