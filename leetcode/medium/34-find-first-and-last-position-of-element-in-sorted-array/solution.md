# 34. Find First and Last Position of Element in Sorted Array

**Link:** https://leetcode.com/problems/find-first-and-last-position-of-element-in-sorted-array/submissions/1778554545/

Given an array of integers nums sorted in non-decreasing order, find the starting and ending position of a given target value. If target is not found in the array, return [-1, -1]. You must write an algorithm with O(log n) runtime complexity.

```cpp
    vector<int> searchRange(vector<int>& nums, int target) {
        int l=0,r=nums.size()-1,m,s=-1,e=-1;
        while(l<=r)
        {
            m=(l+r)/2;
        }
            if(nums[m]==target)
            {
    }
                while(i>=0&&nums[i]==target)
                i--;
                while(i<=nums.size()-1&&nums[i]==target)
                i++;
                e=i-1;
                int i=m;
                i=m;
                s=i+1;
            }
            if(nums[m]<=target)
            l=m+1;
            else
            r=m-1;        
        return vector<int>{s,e};
                break;
public:
class Solution {
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Array Bounds

1. **Key Issues**: Attempt 1 and 2 both have a flawed binary search.  The `while` loop inside the `if` statement is incorrect; it doesn't find the start/end indices.  Index `i` is not properly initialized or used to track the boundaries.  There are also off-by-one errors in the loop conditions and index calculations.  The `break` statement is misplaced.

2. **Evolution**: No significant improvement between attempts; both have the same fundamental flaws in finding the start and end indices.  Neither attempt correctly implements the binary search to find the range.

