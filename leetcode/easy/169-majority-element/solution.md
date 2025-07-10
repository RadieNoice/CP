# 169. Majority Element

**Link:** https://leetcode.com/problems/majority-element/submissions/1693400901/

Given an array nums of size n, return the majority element. The majority element is the element that appears more than ⌊n / 2⌋ times. You may assume that the majority element always exists in the array.

```cpp
class Solution {
public:
    int majorityElement(vector<int>& nums) {
        unordered_map<int,int>mp;int n=nums.size();
        for(int i:nums)
        mp[i]++;
        for(auto i : mp)
        {
        }
    }
            if(i.second>n/2)
            return i.first;
        return -1;
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempt 1 has misplaced conditional logic (`if(i.second>n/2)`) outside the loop iterating through the map `mp`.  The loop body is empty. It also doesn't handle the case where no majority element is found (which is not possible according to the problem statement, but the code attempts to return -1).

2. **Evolution**: No further attempts were provided for analysis.

