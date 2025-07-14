# 560. Subarray Sum Equals K

**Link:** https://leetcode.com/problems/subarray-sum-equals-k/description/

Given an array of integers nums and an integer k, return the total number of subarrays whose sum equals to k. A subarray is a contiguous non-empty sequence of elements within an array.

```cpp
class Solution {
public:
    int subarraySum(vector<int>& nums, int k) {
        for(int i=0;i<n;i++)
        {
        }
        return c;

        int n=nums.size(),c=0;
            for(int j=i;j<n;j++)
            {
            }
    }
            int s=0;
                s+=nums[j];
                if(s==k)
                c++;
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Algorithm Choice

1. **Key Issues**: Attempts 1-6 incorrectly used `unordered_map` to count subarrays.  Attempts 7-12 failed to iterate through all subarrays. Attempts 13-19 had incomplete nested loops and incorrect logic for summing subarray elements.  None correctly implemented a cumulative sum algorithm.

2. **Evolution**: Attempts moved from an incorrect `unordered_map` approach toward a nested loop structure for iterating subarrays. However, attempts consistently lacked correct logic within the nested loops to calculate the subarray sum and count correctly.

