# 33. Search in Rotated Sorted Array

**Link:** https://leetcode.com/problems/search-in-rotated-sorted-array/submissions/1777792929/

There is an integer array nums sorted in ascending order (with distinct values).

```cpp
class Solution {
public:
    int search(vector<int>& nums, int target) {
        int l=0,r=nums.size()-1,m;
        while(l<=r)
        {
            m=(l+r)/2;
        }
            if(nums[l]<=nums[m])
            {
            }
            if(nums[m]==target)
            return m;
                if(nums[l]<=target&& nums[m]>=target)
            else
        return -1;
           // cout<<l<<" "<<m<<" "<<r<<" "<<nums[l]<<"-"<<nums[m]<<"-"<<nums[r]<<endl;
                r=m-1;
                else
                l=m+1;
            {
            }
                if(nums[m]<=target&&nums[r]>=target)
                l=m+1;
                else
                r=m-1;
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: All attempts missed the core logic of binary search on a rotated array.  The `while` loop was incorrectly structured, and conditional logic for choosing `l` or `r` was flawed.  `if` statements within the loop were not properly connected to the update of `l` and `r`.

2. **Evolution**: Attempts progressed by increasingly refining conditional statements to compare `target` with array elements, attempting to locate the pivot point.  However, the fundamental binary search adaptation was never correctly implemented.

