# 1578. Minimum Time to Make Rope Colorful

**Link:** https://leetcode.com/problems/minimum-time-to-make-rope-colorful/submissions/1819440267/

Alice has n balloons arranged on a rope. You are given a 0-indexed string colors where colors[i] is the color of the ith balloon. Alice wants the rope to be colorful. She does not want two consecutive balloons to be of the same color, so she asks Bob for help. Bob can remove some balloons from the rope to make it colorful. You are given a 0-indexed integer array neededTime where neededTime[i] is the time (in seconds) that Bob needs to remove the ith balloon from the rope. Return the minimum time Bob needs to make the rope colorful.

```cpp
class Solution {
public:
    int minCost(string colors, vector<int>& time) {
        int n=colors.size(),t=0;
        for(int i=0;i<n-1;i++)
        {
            if(colors[i]==colors[i+1]){
        }
    }
            t+=min(time[i],time[i+1]);
        return t;
            }
            time[i+1]=max(time[i],time[i+1]);
};
```
