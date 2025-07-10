# 1. Two Sum

**Link:** https://leetcode.com/problems/two-sum/submissions/1693361148/

Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target. You may assume that each input would have exactly one solution, and you may not use the same element twice. You can return the answer in any order.

```cpp
            break;
        }
        return x;
    //     unordered_map<int,int>mp;int n=nums.size();
    //     vector<int>arr;
    //     for(int i=0;i<n;i++)
    //     {
    //         int x=nums[i];
    //         int y=target-x;
    //         if(mp.find(y)!=mp.end())
    //         {
    //             arr.emplace_back(i);
    //             arr.emplace_back(mp[y]);
    //         }
    //         mp[x]=i;
    //     }
    //     return arr;
    }

};
            x.emplace_back(k);
            if(x.size()==2)
        vector<int>x;
        for(int k=0;k<n;k++)
        {
            if(nums[i]==copy[k]||nums[j]==copy[k])
        }
            break;
            j--;
            if (x==target)
            if(x>target)
            i++;
            if(x<target)
            int x=nums[i]+nums[j];
        {
        while(nums[i]+nums[j]!=target)
        int i=0,j=nums.size()-1,n=nums.size();
        sort(nums.begin(),nums.end());
        vector<int>copy(nums.begin(),nums.end());
    vector<int> twoSum(vector<int>& nums, int target) {
public:
class Solution {
```
