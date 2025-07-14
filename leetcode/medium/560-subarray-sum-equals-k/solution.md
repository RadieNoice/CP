# 560. Subarray Sum Equals K

**Link:** https://leetcode.com/problems/subarray-sum-equals-k/submissions/1697723846/

Given an array of integers nums and an integer k, return the total number of subarrays whose sum equals to k. A subarray is a contiguous non-empty sequence of elements within an array.

```cpp
        // int n=nums.size(),c=0;
        // for(int i=0;i<n;i++)
        // {
        //     int s=0;
        //     for(int j=i;j<n;j++)
        //     {
        //         s+=nums[j];
        //         if(s==k)
        //         c++;
        //     }
        {
        }
            if(mp.contains(ps-k))
            mp[ps]++;
            {
            }
            ps+=i;
        // }
                c+=mp[ps-k];
        for(int i:nums)
        int ps=0,c=0;
        mp[0]=1;
        unordered_map<int,int>mp;
    int subarraySum(vector<int>& nums, int k) {
public:
class Solution {
        return c;
        // return c;
```

## Mistake Analysis

TAGS: Logic Error, Algorithm Choice, Data Structure

1. **Key Issues**: Attempts 1-3 all contain a flawed implementation of the prefix sum technique.  The `if` condition incorrectly checks for the presence of `ps-k` instead of incrementing the count based on its occurrences. The code also has syntax and structural problems, such as misplaced code blocks.

2. **Evolution**: Attempt 3 shows a slight improvement by attempting to add `mp[ps-k]` to `c`. However, this is still logically incorrect due to the mishandling of the prefix sum. The core algorithm remains flawed across all attempts.

