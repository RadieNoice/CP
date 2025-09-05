# 287. Find the Duplicate Number

**Link:** https://leetcode.com/problems/find-the-duplicate-number/submissions/1760407328/

Given an array of integers nums containing n + 1 integers where each integer is in the range [1, n] inclusive. There is only one repeated number in nums, return this repeated number. You must solve the problem without modifying the array nums and using only constant extra space.

```cpp
class Solution {
public:
    int findDuplicate(vector<int>& nums) {
        // sort(nums.begin(),nums.end());
        // for(int i=1;i<nums.size();i++)
        // {
        //     if(nums[i]==nums[i-1])
        //     return nums[i];
        // }
        // return -1;
        int i=0,n=nums.size();
        while(true)
        {
            if(nums[i]==-1)
        }
            return i;
            else
            {
                int j=nums[i];
            }
    }
                nums[i]=-1;
                i=j;
};
```

## Mistake Analysis

TAGS: Loop Logic, Logic Error, Conditional Logic

1. **Key Issues**: Attempt 1 and 2 both have incomplete loops (`while(true)` without a break condition) and incorrect logic for finding the duplicate.  Neither correctly uses the `nums[i] = -1` modification to track visited elements. Attempt 2 improves by using `nums[i]` to index instead of a fixed `i`.

2. **Evolution**:  Attempt 2 shows some understanding of using the array elements to traverse. Both attempts fail to implement a proper cycle detection algorithm for finding duplicates and suffer from incomplete and flawed loop constructs.

