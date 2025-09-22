# 34. Find First and Last Position of Element in Sorted Array

**Link:** https://leetcode.com/problems/find-first-and-last-position-of-element-in-sorted-array/

Given an array of integers nums sorted in non-decreasing order, find the starting and ending position of a given target value. If target is not found in the array, return [-1, -1]. You must write an algorithm with O(log n) runtime complexity.

```cpp
        // if(nums[l]==target&&nums[r]==target)
        // return vector<int>{l,r};
        while(l<=r)
        {
            m=(l+r)/2;
            if(nums[m]<target)
            s=m;
            if(nums[m]<target)
            l=m+1;
            else
            r=m-1;        
        }
        l=0;r=nums.size()-1;
        while(l<=r)
        {
            m=(l+r)/2;
            if(nums[m]>target)
            e=m;
            if(nums[m]<=target)
            l=m+1;
            else
            r=m-1;
        }
        if(s!=-1&&e!=-1){
        s++;e--;
        }

        return vector<int>{s,e};
        int l=0,r=nums.size()-1,m,s=-1,e=-1;
    vector<int> searchRange(vector<int>& nums, int target) {
public:
class Solution {
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-4 suffer from incorrect conditional logic within binary search loops.  The `if` and `else if` conditions are improperly structured, leading to incorrect index updates. Attempt 5 uses two separate binary searches but lacks logic to handle finding the first and last occurrences correctly.

2. **Evolution**:  Attempts show a gradual refinement of the binary search logic, but the core conditional error persists until the final attempt, which is still unfinished and lacks the necessary post-processing to return the correct range.

