# 56. Merge Intervals

**Link:** https://leetcode.com/problems/merge-intervals/submissions/1719747098/

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
