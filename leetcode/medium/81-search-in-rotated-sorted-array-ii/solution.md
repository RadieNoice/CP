# 81. Search in Rotated Sorted Array II

**Link:** https://leetcode.com/problems/search-in-rotated-sorted-array-ii/submissions/1777807123/

There is an integer array nums sorted in non-decreasing order (not necessarily with distinct values).

```cpp
            if(nums[m]==target)
            return true;
            if(nums[l]<=nums[m])
            {
                if(nums[l]<=target&&nums[m]>=target)
            }
                r=m-1;
                else
                l=m+1;
            else
            {
                if(nums[m]<=target&&nums[r]>=target)
                l=m+1;
                else
            if(nums[l]==nums[m]&&nums[m]==nums[r])
            {
                l++;r--;
            }
                continue;
                r=m-1;
            }
        }
            int m=(l+r)/2;
        {
        while(l<=r)
        int l=0,r=nums.size()-1;
```

## Mistake Analysis

TAGS: Logic Error, Conditional Logic, Loop Logic

1. **Key Issues**: Attempts 1-3 have incomplete conditional logic within the `while` loop, lacking the crucial `l=m+1` or `r=m-1` assignments in several branches. Attempts 4-6 partially address this but introduce errors in handling duplicate values (`nums[l]==nums[m]&&nums[m]==nums[r]`) which is incomplete. The loop termination condition and the placement of `int m = (l+r)/2` are also problematic.

2. **Evolution**: Attempts progressively fix parts of the conditional logic. However, none correctly handle the case of duplicate elements to shrink the search space effectively within the rotated sorted array.

