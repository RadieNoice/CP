# 74. Search a 2D Matrix

**Link:** https://leetcode.com/problems/search-a-2d-matrix/submissions/1720399197/

You are given an m x n integer matrix matrix with the following two properties: Each row is sorted in non-decreasing order. The first integer of each row is greater than the last integer of the previous row. Given an integer target, return true if target is in matrix or false otherwise. You must write a solution in O(log(m * n)) time complexity.

```cpp
class Solution {
public:
    bool searchMatrix(vector<vector<int>>& nums, int t) {
        int n=nums.size(),m=nums[0].size();
        for(vector<int>i:nums)
        {
            if(i[m-1]>=t)
            {
                for(int k:i)
                {
                    if(k==t)
                    return true;
                }
                return false;
            }
        }
        return false;
    }
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: All attempts have incomplete or incorrect conditional logic within nested loops. They fail to correctly iterate through rows based on target value and check for target within each row.  Unclosed loops and improper return statements compound the problem.

2. **Evolution**:  Attempts gradually corrected the index used (`n` to `m`). However, the fundamental flaw in conditional logic and loop structure remained unfixed.  No attempt successfully implemented a binary search or efficient search strategy.

