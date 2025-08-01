# 56. Merge Intervals

**Link:** https://leetcode.com/problems/merge-intervals/submissions/1719746849/

Given an array of intervals where intervals[i] = [starti, endi], merge all overlapping intervals, and return an array of the non-overlapping intervals that cover all the intervals in the input.

```cpp
class Solution {
public:
    vector<vector<int>> merge(vector<vector<int>>& nums) {
        sort(nums.begin(),nums.end(),[](vector<int>&a,vector<int>&b){return a[0]<b[0];});
        for(int i=0;i<nums.size();i++)
        {
        }
        return ans;
            if(y>=nums[i][0])
            {
            }
        int x=nums[0][0];int y=nums[0][1];vector<vector<int>>ans;
                y=max(y,nums[i][1]);
            else
            {
                ans.push_back({x,y});
            }
    }
                x=nums[i][0];y=nums[i][1];
        ans.push_back({x,y});
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**:  Attempts 1-11 had unclosed loops and incorrect conditional logic for merging intervals. `ans` was undeclared. Attempt 12's loop iterates one time too many and has incorrect logic for merging intervals.  The core logic for merging was missing.

2. **Evolution**: Attempts incrementally added code, mostly unsuccessfully correcting syntax and attempting to implement the merge logic.  Attempt 12 is the first to approach a complete loop. However, the conditionals and logic for interval merging is still faulty.

