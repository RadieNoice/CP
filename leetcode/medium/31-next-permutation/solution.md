# 31. Next Permutation

**Link:** https://leetcode.com/problems/next-permutation/submissions/1695503905/

A permutation of an array of integers is an arrangement of its members into a sequence or linear order.

```cpp
class Solution {
public:
    void nextPermutation(vector<int>& nums) {

        int n= nums.size(),t=-1;
        for(int i=n-2;i>=0;i--)
        {
            if(nums[i+1]>nums[i])
            {
        }
        
            }
                t=i;break;
        if(t==-1)
        sort(nums.begin(),nums.end());
        else
        {
            for(int i=n-1;i>t;i--)
        }
            {
                if(nums[i]>nums[t]){
            }
    }
                swap(nums[i],nums[t]);
                break;}
            sort(nums.begin()+t+1,nums.end());
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-4 had incomplete or incorrect loops and conditional logic for finding the pivot point for the permutation. Attempts 5-19 had syntax errors (missing semicolons, incorrect `if` statements, dangling `else`) and logical errors in finding and swapping elements. Attempt 20-21 had correct logic but missed handling of the case where the input array is sorted in descending order.

2. **Evolution**: The attempts progressively moved towards the correct algorithm for finding the next permutation.  However, syntax and logical errors in implementing the `upper_bound` and swapping mechanism hindered progress until the final attempt which correctly identifies the pivot and swaps elements before sorting the remaining sub-array.

