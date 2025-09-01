# 26. Remove Duplicates from Sorted Array

**Link:** https://leetcode.com/problems/remove-duplicates-from-sorted-array/submissions/1755733968/

Given an integer array nums sorted in non-decreasing order, remove the duplicates in-place such that each unique element appears only once. The relative order of the elements should be kept the same. Then return the number of unique elements in nums. Consider the number of unique elements of nums to be k, to get accepted, you need to do the following things: Change the array nums such that the first k elements of nums contain the unique elements in the order they were present in nums initially. The remaining elements of nums are not important as well as the size of nums. Return k. Custom Judge: The judge will test your solution with the following code: int[] nums = [...]; // Input array int[] expectedNums = [...]; // The expected answer with correct length int k = removeDuplicates(nums); // Calls your implementation assert k == expectedNums.length; for (int i = 0; i < k; i++) { assert nums[i] == expectedNums[i]; } If all assertions pass, then your solution will be accepted.

```cpp
            i++;
            }
                //cout<<t<<" "<<j<<endl;
                }
        }
        for(int i:nums)
                j++;
                nums[j]=nums[i];
                t=nums[i];
                {
                if(t!=nums[i])
            {
            else
            }
        cout<<i<<" ";
        return j;
        // int i=0,n=nums.size();
        // for(int j=1;j<n;j++)
            {
                j=i;
        {
            if(j==-1 && t==nums[i])
        int n=nums.size(),i=1,j=1,t=nums[0];
        while(i<n)
    int removeDuplicates(vector<int>& nums) {
public:
class Solution {
        // {
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-6 had incomplete loops and incorrect return values. Attempts 7-44 struggled with conditional logic for duplicate detection and in-place modification, often resulting in incorrect array manipulation and off-by-one errors.  The `k` variable was often misused to track duplicates.

2. **Evolution**: The attempts show a gradual progression toward a correct two-pointer approach.  Debugging attempts (outputting intermediate values) appeared in later attempts, indicating a shift in debugging strategy.  However, the core logic errors persisted until a closer approximation of the two-pointer solution was reached in the final attempts.

