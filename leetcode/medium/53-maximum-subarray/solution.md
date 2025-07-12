# 53. Maximum Subarray

**Link:** https://leetcode.com/problems/maximum-subarray/submissions/1695269375/

Given an integer array nums, find the subarray with the largest sum, and return its sum.

```cpp
class Solution {
public:
    int maxSubArray(vector<int>& nums) {
        int ms=INT_MIN,cs=0;
        for(int i:nums)
        {
            cs+=i;
        }
    }
            ms=max(cs,ms);
        return ms;
            if(cs<0)
            cs=0;
};
```
