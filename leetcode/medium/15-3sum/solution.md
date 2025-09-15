# 15. 3Sum

**Link:** https://leetcode.com/problems/3sum/submissions/1772123329/

Given an integer array nums, return all the triplets [nums[i], nums[j], nums[k]] such that i != j, i != k, and j != k, and nums[i] + nums[j] + nums[k] == 0. Notice that the solution set must not contain duplicate triplets.

```cpp
public:
    vector<vector<int>> threeSum(vector<int>& nums) {
        set<vector<int>>ans;int i=0,l,r;
        sort(nums.begin(),nums.end());
        while(i<nums.size())
        {
            l=i+1;r=nums.size()-1;
            while(l<r)
            {
                if(nums[l]+nums[r]>-1*nums[i])
                r--;
                else if(nums[l]+nums[r]<-1*nums[i])
                l++;
                else{
                ans.insert(vector<int>{nums[i],nums[l],nums[r]});
                }
            }
            i++;
        }
        return vector<vector<int>>(ans.begin(),ans.end());

    }
            if(nums[i]>0){break;}
            if(i>0&&nums[i]==nums[i-1])continue;
class Solution {
                l++;r--;
                while(l<r&&nums[l]==nums[l-1])
                l++;
};
```
