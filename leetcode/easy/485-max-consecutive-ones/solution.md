# 485. Max Consecutive Ones

**Link:** https://leetcode.com/problems/max-consecutive-ones/description/

Given a binary array nums, return the maximum number of consecutive 1's in the array.

```cpp
class Solution {
public:
    int findMaxConsecutiveOnes(vector<int>& nums) {
        int n=nums.size(), ms=0,s=0;
        for(int i=0;i<n;i++)
        {
            if(nums[i]==1){
            s++;
            ms=max(s,ms);
            }
            else
            s=0;
        }
        return ms;
        // int ms=0,cs=0;
        // for(int i: nums)
        // {
        //     if(i==1)
        //     {
        //         cs++;
        //         ms=max(cs,ms);
        //     }
        //     else
        //     cs=0;
        // }
        // return ms;
        // nums.emplace_back(0);
        // int n=nums.size(),c=0,x=0;
```
