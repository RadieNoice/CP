# Q2. How Many Numbers Are Smaller Than the Current Number

**Link:** https://leetcode.com/problems/how-many-numbers-are-smaller-than-the-current-number/submissions/1845619752/

Given the array nums, for each nums[i] find out how many numbers in the array are smaller than it. That is, for each nums[i] you have to count the number of valid j's such that j != i and nums[j] < nums[i]. Return the answer in an array.

```cpp
class Solution {
public:
    vector<int> smallerNumbersThanCurrent(vector<int>& nums) {
        unordered_map<int,int>mp;
        for(int i=0;i<nums.size();i++){
                mp[nums[i]]=i;
    }
        return ans;
        vector<int>ans;
        for(int i=0;i<nums.size();i++)
        ans.push_back(mp[cpy[i]]);
        vector<int>cpy(nums);
        sort(nums.begin(),nums.end());
        }
            if(!mp.count(nums[i]))
};
```
