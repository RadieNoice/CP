# 74. Search a 2D Matrix

**Link:** https://leetcode.com/problems/search-a-2d-matrix/submissions/1720405386/

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
                return false;
            }
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌for(int·‌k:i)
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌{
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌if(k==t)
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌return·‌true;
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌}
        }
        return false;
    }
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: All attempts have an incomplete binary search implementation within the outer loop.  The `while` loop lacks the core binary search logic (updating `j` and `k` correctly). Conditional logic for adjusting `j` and `k` is also flawed across attempts.  The initial check `i[m-1]>=t` is incorrect; it prematurely exits.

2. **Evolution**: Attempts 1-4 show some minor variations in conditional logic, but never correct the fundamental binary search and outer loop issues. None attempt to iterate through rows, only to search a row.

