# Q3. Find All Numbers Disappeared in an Array

**Link:** https://leetcode.com/problems/find-all-numbers-disappeared-in-an-array/description/

Given an array nums of n integers where nums[i] is in the range [1, n], return an array of all the integers in the range [1, n] that do not appear in nums.

```cpp
class Solution {
public:
    vector<int> smallerNumbersThanCurrent(vector<int>& nums) {
        vector<int>cpy(nums);
        sort(nums.begin(),nums.end());
        unordered_map<int,int>mp;
        for(int i=0;i<nums.size();i++){
            if(!mp.count(nums[i]))
                mp[nums[i]]=i;
        }
        vector<int>ans;
        for(int i=0;i<nums.size();i++)
        ans.push_back(mp[cpy[i]]);
        return ans;
    }
};
```
