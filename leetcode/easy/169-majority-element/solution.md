# 169. Majority Element

**Link:** https://leetcode.com/problems/majority-element/submissions/1701141936/

Given an array nums of size n, return the majority element. The majority element is the element that appears more than ⌊n / 2⌋ times. You may assume that the majority element always exists in the array.

```cpp
class Solution {
public:
    int majorityElement(vector<int>& nums) {
        // unordered_map<int,int>mp;int n=nums.size();
        // for(int i:nums)
        // mp[i]++;
        // for(auto i : mp)
        // {
        //     if(i.second>n/2)
        //     return i.first;
        // }
        // return -1;
        int ele,c=0;
        for(int i=0;i<nums.size();i++)
        {
            if(c==0){
        }
    }
            ele=nums[i];
            else
            {
                if (ele==nums[i])
            }
                c++;
                else c--;
            }
            c++;
        return ele;
```
