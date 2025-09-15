# 15. 3Sum

**Link:** https://leetcode.com/problems/3sum/submissions/1772127544/

Given an integer array nums, return all the triplets [nums[i], nums[j], nums[k]] such that i != j, i != k, and j != k, and nums[i] + nums[j] + nums[k] == 0. Notice that the solution set must not contain duplicate triplets.

```cpp
class Solution {
public:
    vector<vector<int>> threeSum(vector<int>& nums) {
        vector<vector<int>>ans;int i=0,l,r;
        sort(nums.begin(),nums.end());
        for(;i<nums.size();i++)
        {
            if(nums[i]>0){break;}
            if(i>0&&nums[i]==nums[i-1])continue;
            l=i+1;r=nums.size()-1;
            while(l<r)
            {
                if(nums[l]+nums[r]>-nums[i])
                r--;
                else if(nums[l]+nums[r]<-nums[i])
                l++;
                else{
                    ans.emplace_back(vector<int>{nums[i],nums[l],nums[r]});
                    l++;r--;
                    while(l<r&&nums[l]==nums[l-1])
                    l++;
                    }
            }
        }
        return ans;

    }
};
```

## Mistake Analysis

TAGS: Loop Logic, Conditional Logic, Edge Cases

1. **Key Issues**: Attempts 1-7 had incorrect `while` loop conditions for duplicate handling of `r`, sometimes decrementing `r` when it should be incremented. Attempts 8-11 corrected this. Attempt 10 and 11 unnecessarily omitted `i++` in the `while` loop for `i`.

2. **Evolution**: The code evolved to correctly handle duplicate numbers and improve efficiency by moving `i++` outside the inner `while` loop.  The final attempts correctly skip duplicates and use a `for` loop instead of `while`.

