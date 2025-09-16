# 42. Trapping Rain Water

**Link:** https://leetcode.com/problems/trapping-rain-water/submissions/1772517680/

Given n non-negative integers representing an elevation map where the width of each bar is 1, compute how much water it can trap after raining.

```cpp
class Solution {
public:
    int trap(vector<int>& nums) {
        int n=nums.size(),t=0,count=0;
        vector<int>ml(n),mr(n);
        for(int i=1;i<n;i++)
        {
        }
        ml[0]=0;
            ml[i]=max(nums[i-1],t);
            t=ml[i];
        return count;
        for(int i=n-2;i>=0;i--)
        {
            mr[i]=max(nums[i+1],t);
        }
            t=mr[i];
        t=0;mr[n-1]=0;
        for(int i=0;i<n;i++)
        {
            int min_h=min(ml[i],mr[i]);
        }
    }
                count+=min_h-nums[i];
            if(min_h-nums[i]>0)
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Array Bounds

1. **Key Issues**: Attempts 1-8 had incomplete or incorrect loops for calculating left/right maxes (`ml`, `mr`).  Attempt 9 correctly calculated `ml`, `mr` but lacked a loop to sum trapped water. `ml[0]` and `mr[n-1]` were incorrectly initialized.

2. **Evolution**:  Attempts progressed toward correctly computing left and right maximums. Attempt 9 finally implemented the core logic of finding the minimum height and calculating trapped water but contained some minor issues that could be easily fixed.

