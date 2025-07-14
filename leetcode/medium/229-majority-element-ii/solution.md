# 229. Majority Element II

**Link:** https://leetcode.com/problems/majority-element-ii/submissions/1697778249/

Given an integer array of size n, find all elements that appear more than ⌊ n/3 ⌋ times.

```cpp
class Solution {
public:
    vector<int> majorityElement(vector<int>& nums) {
        int n=nums.size();vector<int>ans;
        n/=3;
        cout<<n;
        unordered_map<int,int>mp;
        for(int i:nums){
        mp[i]++;
        for(auto i:mp)
        {
            if(i.second>n)
            ans.emplace_back(i.first);
        }
        return ans;
    }
        }
};
```

## Mistake Analysis

TAGS: Loop Logic, Logic Error, Conditional Logic

1. **Key Issues**: Attempt 1 places the inner `for` loop iterating through the map *inside* the main loop iterating through `nums`. This leads to redundant checks and incorrect counts. The condition `i.second > n` is correct, but the loop placement is flawed.

2. **Evolution**: No further attempts were provided to analyze improvement.  The provided code has a fundamental logic error in loop placement, requiring restructuring rather than incremental fixes.

