# 15. 3Sum

**Link:** https://leetcode.com/problems/3sum/submissions/

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
