# 287. Find the Duplicate Number

**Link:** https://leetcode.com/problems/find-the-duplicate-number/submissions/1720391345/

Given an array of integers nums containing n + 1 integers where each integer is in the range [1, n] inclusive. There is only one repeated number in nums, return this repeated number. You must solve the problem without modifying the array nums and using only constant extra space.

```cpp
class Solution {
public:
    int findDuplicate(vector<int>& nums) {
        sort(nums.begin(),nums.end());
        for(int i=1;i<nums.size();i++)
        {
            if(nums[i]==nums[i-1])
        }
    }
            return nums[i];
        return -1;
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Array Bounds

1. **Key Issues**: Attempt 1 & 2: Missing return statement inside the loop and after the loop, leading to undefined behavior. Attempt 3:  Incorrect loop termination condition (`i < nums.size()`) causing potential array bounds error;  `nums[i]` might be accessed outside the array.  All attempts lack a return statement if a duplicate is found within the loop.

2. **Evolution**: Attempts moved towards a correct loop condition but failed to address the missing return statements and the potential for array out-of-bounds issues in the loop condition.

