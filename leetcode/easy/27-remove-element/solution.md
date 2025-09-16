# 27. Remove Element

**Link:** https://leetcode.com/problems/remove-element/submissions/1772597236/

Given an integer array nums and an integer val, remove all occurrences of val in nums in-place. The order of the elements may be changed. Then return the number of elements in nums which are not equal to val. Consider the number of elements in nums which are not equal to val be k, to get accepted, you need to do the following things: Change the array nums such that the first k elements of nums contain the elements which are not equal to val. The remaining elements of nums are not important as well as the size of nums. Return k. Custom Judge: The judge will test your solution with the following code: int[] nums = [...]; // Input array int val = ...; // Value to remove int[] expectedNums = [...]; // The expected answer with correct length. // It is sorted with no values equaling val. int k = removeElement(nums, val); // Calls your implementation assert k == expectedNums.length; sort(nums, 0, k); // Sort the first k elements of nums for (int i = 0; i < actualLength; i++) { assert nums[i] == expectedNums[i]; } If all assertions pass, then your solution will be accepted.

```cpp
        // int n=nums.size(),l=0,r=0;
        while(l<n)
        {
            if(nums[l]!=val)
        }
            if(nums[i]==val)
        }
            {
                r=i;break;
            }
        l=r+1;
            {
                swap(nums[l],nums[r]);
            }
                r++;
            l++;
        return r;
        {
        for(int i=0;i<n;i++)
        int n=nums.size(),l,r=-1;
public:
    int removeElement(vector<int>& nums, int val) {
class Solution {
        if(r==-1)
        return n;
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: All attempts have incomplete or incorrect logic for swapping elements.  The `if` conditions are missing crucial parts for correctly identifying and moving non-`val` elements.  The loops don't effectively iterate and update `l` and `r`.

2. **Evolution**: Attempts 2 and 3 show some minor syntax improvements (return value) but the core logic flaws remain unaddressed. No significant progress toward a correct solution.

