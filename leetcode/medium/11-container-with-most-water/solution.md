# 11. Container With Most Water

**Link:** https://leetcode.com/problems/container-with-most-water/submissions/1751829486/

You are given an integer array height of length n. There are n vertical lines drawn such that the two endpoints of the ith line are (i, 0) and (i, height[i]). Find two lines that together with the x-axis form a container, such that the container contains the most water. Return the maximum amount of water a container can store. Notice that you may not slant the container.

```cpp
class Solution {
public:
    int maxArea(vector<int>& num) {
        int n=num.size(),i=0,j=n-1,area=0;
        while(i<j)
        {
        }
            int cur_area=min(num[i],num[j])*(j-i);
    }
        return area;
            area=max(area,cur_area);
            cout<<cur_area;
            if(num[i]<num[j])
            i++;
            else
            j--;
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-6 had incomplete or incorrect `while` loops and conditional logic for updating `i` and `j`. Attempt 7-9 had the correct loop structure, but `cur_area` calculation or pointer adjustment was flawed.

2. **Evolution**: The code gradually moved toward a two-pointer approach.  The major flaw (incorrect area calculation and pointer update) was only corrected in the final attempt (though it still has a `cout` statement).

