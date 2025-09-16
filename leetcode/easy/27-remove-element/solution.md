# 27. Remove Element

**Link:** https://leetcode.com/problems/remove-element/submissions/1772589071/

Given an integer array nums and an integer val, remove all occurrences of val in nums in-place. The order of the elements may be changed. Then return the number of elements in nums which are not equal to val. Consider the number of elements in nums which are not equal to val be k, to get accepted, you need to do the following things: Change the array nums such that the first k elements of nums contain the elements which are not equal to val. The remaining elements of nums are not important as well as the size of nums. Return k. Custom Judge: The judge will test your solution with the following code: int[] nums = [...]; // Input array int val = ...; // Value to remove int[] expectedNums = [...]; // The expected answer with correct length. // It is sorted with no values equaling val. int k = removeElement(nums, val); // Calls your implementation assert k == expectedNums.length; sort(nums, 0, k); // Sort the first k elements of nums for (int i = 0; i < actualLength; i++) { assert nums[i] == expectedNums[i]; } If all assertions pass, then your solution will be accepted.

```cpp
class Solution {
public:
    int removeElement(vector<int>& nums, int val) {
        int n=nums.size(),l=0,r=0;
        while(l<nums.size())
        {
            if(nums[l]==val)
        }
            {
                swap(nums[l],nums[r]);
            }
                r++;
            l++;
        return n-r;
    }
        reverse(nums.begin(),nums.end());
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: All attempts lacked complete conditional logic within the while loop.  The `if` statement checking for `nums[l] == val` was never completed, causing incorrect swapping and loop termination.  Incorrect return values were also used.

2. **Evolution**: Attempts progressed towards using two pointers (`l` and `r`), but the core logic error persisted until attempt 23 (partially).  Attempts 19-23 added `reverse`, but this wasn't necessary for solving the problem.  Attempts 6-10 tried to adjust loop bounds but incorrectly.

