# 35. Search Insert Position

**Link:** https://leetcode.com/problems/search-insert-position/description/

Given a sorted array of distinct integers and a target value, return the index if the target is found. If not, return the index where it would be if it were inserted in order. You must write an algorithm with O(log n) runtime complexity.

```cpp
class Solution {
public:
    int searchInsert(vector<int>& nums, int target) {
       int m=0,n=nums.size()-1; 
       while(m<=n)
       {
            else if(nums[a]>target)
       }
    }
            int a=(m+n)/2;
            n=a-1;
            if(nums[a]==target)
            return a;
            else 
            m=a+1;
       return m;
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempt 1 and 2 are nearly identical and incomplete.  The `else if` condition is dangling and lacks a closing brace for the `while` loop. The binary search logic is flawed; `n` should be updated to `a` in some cases.  The final return value `m` isn't always correct if the target is not found.

2. **Evolution**: No actual evolution occurred between attempts; they're the same incomplete code.

