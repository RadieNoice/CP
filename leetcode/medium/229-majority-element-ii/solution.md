# 229. Majority Element II

**Link:** https://leetcode.com/problems/majority-element-ii/submissions/1697776310/

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

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-3 incorrectly used `accumulate` to find the array size and had misplaced code within loops, failing to add elements to `ans`. Attempts 4-6 had the same misplaced code. Attempt 7 had a `>` instead of `>=` in the conditional.

2. **Evolution**: The code gradually corrected the use of `accumulate` (replacing it with `nums.size()`), and the placement of `ans.emplace_back()`, showing improvement in loop and conditional logic.  The final error (incorrect comparison) remains.

