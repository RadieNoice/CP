# 167. Two Sum II - Input Array Is Sorted

**Link:** https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/submissions/1771016535/

Given a 1-indexed array of integers numbers that is already sorted in non-decreasing order, find two numbers such that they add up to a specific target number. Let these two numbers be numbers[index1] and numbers[index2] where 1 <= index1 < index2 <= numbers.length. Return the indices of the two numbers, index1 and index2, added by one as an integer array [index1, index2] of length 2. The tests are generated such that there is exactly one solution. You may not use the same element twice. Your solution must use only constant extra space.

```cpp
class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int t) {
        int l=0,r=nums.size()-1;
        while(l<r)
        {
            if(nums[l]+nums[r]==t)
        }
    }
            return vector<int>{l+1,r+1};
            else if(nums[l]+nums[r]>t)
            r--;
            else 
            l++;
        return vector<int>{-1,-1};
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-7 all had a missing `return` statement within the `while` loop.  The `else if` and `else` blocks were incorrectly decrementing/incrementing `l` in some attempts.  The final `return {-1,-1}` was unreachable.  Indices were not incremented correctly before return.


2. **Evolution**: Attempts progressively corrected the `l` increment/decrement issue (Attempt 6 and 7 got this correct). Attempt 4 corrected return values to indices, while attempt 5 and onwards corrected to 1-based indexing (as required by problem).  The core loop logic error remained unfixed until explicitly shown in the corrected code (not provided in the prompt).

