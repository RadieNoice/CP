# 229. Majority Element II

**Link:** https://leetcode.com/problems/majority-element-ii/description/

Given an integer array of size n, find all elements that appear more than ⌊ n/3 ⌋ times.

```cpp
class Solution {
public:
    vector<int> majorityElement(vector<int>& nums) {
        int n=nums.size();vector<int>ans;
        n=n/3;
        unordered_map<int,int>mp;
        for(int i:nums)
        mp[i]++;
        for(auto i:mp)
        {
            if(i.second>n)
        }
    }
            ans.emplace_back(i.first);
        return ans;
        cout<<n;
};
```
