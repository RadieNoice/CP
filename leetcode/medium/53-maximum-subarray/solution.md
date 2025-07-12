# 53. Maximum Subarray

**Link:** https://leetcode.com/problems/maximum-subarray/submissions/1695269283/

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

## Mistake Analysis

TAGS: Logic Error, Loop Logic

1. **Key Issues**: Attempt 1 and 2 both incorrectly calculate the maximum subarray sum.  They accumulate the total sum of the array in `cs` but fail to reset `cs` when encountering a negative subarray sum. The `if(cs<0) cs=0;` statement in attempt 2 is misplaced, outside the loop.

2. **Evolution**: No significant improvement. Attempt 2 introduces a misplaced conditional, not fixing the core logic flaw.  Neither attempt correctly implements Kadane's algorithm or a similar approach to track maximum subarray sums.

