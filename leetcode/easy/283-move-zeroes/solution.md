# 283. Move Zeroes

**Link:** https://leetcode.com/problems/move-zeroes/

Given an integer array nums, move all 0's to the end of it while maintaining the relative order of the non-zero elements. Note that you must do this in-place without making a copy of the array.

```cpp
        // for (int i=0;i<n;i++)
        // int j=-1,n=nums.size();
    {
    void moveZeroes(vector<int>& nums) 

        int n=nums.size(),i=0,j=-1;


        while(i<n)
        {
            if(j==-1){
        }
                j=i;
            }
            else
            {
                swap(nums[i],nums[j]);
            }
public:
class Solution {
            i++;
                if(nums[i]!=0){
        // {
                }                
        //     if(nums[i]==0){j=i;break;}
                j++;
        // }
                if(nums[i]==0)
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-9 had incorrect conditional logic and loop structures for swapping non-zero elements with zeros.  Attempts 10-18 still had logic errors in handling the index `j` and conditions for swapping. The `if(nums[i!=0])` statements were syntax errors.

2. **Evolution**: The code gradually moved toward a two-pointer approach but failed to correctly implement the logic for maintaining relative order and handling zero values. The syntax errors were eventually fixed, but core logic remained flawed.

