# 75. Sort Colors

**Link:** https://leetcode.com/problems/sort-colors/submissions/1693395222/

Given an array nums with n objects colored red, white, or blue, sort them in-place so that objects of the same color are adjacent, with the colors in the order red, white, and blue. We will use the integers 0, 1, and 2 to represent the color red, white, and blue, respectively. You must solve this problem without using the library's sort function.

```cpp
        
        }
                swap(nums[k],nums[j]);
            }
                k--;
            else
            {
                j++;
            }
            {
            else if(nums[j]==2)
            }
            j++;
            i++;
            swap(nums[i],nums[j]);
            if(nums[j]==0){
        {
        while(j<=k)
        int i=0,n=nums.size(),k=n-1,j=0;
    void sortColors(vector<int>& nums) {
public:
class Solution {
        //D
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-8 had incomplete or incorrect conditional logic within nested loops for three-way partitioning.  Incorrect loop conditions and `swap` usage prevented correct sorting. Attempt 9-12 improved loop condition but still had incorrect `swap` indexing.

2. **Evolution**: The attempts gradually refined the loop structure and conditional logic for a three-way partitioning approach, though fixing the `swap` logic came later.  The final attempt shows a rudimentary understanding of the algorithm but still needs correction of swap logic.

