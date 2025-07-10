# 1. Two Sum

**Link:** https://leetcode.com/problems/two-sum/

Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target. You may assume that each input would have exactly one solution, and you may not use the same element twice. You can return the answer in any order.

```cpp
class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target) {
        vector<int>copy(nums.begin(),nums.end());
        sort(nums.begin(),nums.end());
        int i=0,j=nums.size()-1,n=nums.size();
        while(nums[i]+nums[j]!=target)
        {
            int x=nums[i]+nums[j];
            if(x<target)
            i++;
            if(x>target)
            j--;
            if (x==target)
            break;
        }
        vector<int>x;
        for(int k=0;k<n;k++)
        {
            if(nums[i]==copy[k]||nums[j]==copy[k])
            x.emplace_back(k);
            if(x.size()==2)
            break;
        }
```
