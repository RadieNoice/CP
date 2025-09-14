# 73. Set Matrix Zeroes

**Link:** https://leetcode.com/problems/set-matrix-zeroes/submissions/1695538407/

Given an m x n integer matrix matrix, if an element is 0, set its entire row and column to 0's. You must do it in place.


## Mistake Analysis

TAGS: Logic Error, Space Complexity

1. **Key Issues**: Attempt 1 uses an extra vector `z` to store zero coordinates, leading to O(m*n) space complexity.  It also double-counts zeroing rows and columns, potentially overwriting values. The code is also incomplete, missing a closing brace.

2. **Evolution**: No further attempts were provided to analyze.  A better approach would use the first row and column to track zeroes, in-place, achieving O(1) space complexity.

