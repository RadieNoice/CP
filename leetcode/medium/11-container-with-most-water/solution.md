# 11. Container With Most Water

**Link:** https://leetcode.com/problems/container-with-most-water/submissions/1751829627/

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
            if(num[i]<num[j])
            i++;
            else
            j--;
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempt 1 has unclosed brackets causing a syntax error. The `while` loop body is missing.  The `max` function to update `area` is misplaced, within the `if-else` block instead of after calculating `cur_area`.

2. **Evolution**: No evolution is shown as only one incomplete attempt is provided.  The code needs to properly iterate, calculate the area, and update the maximum area accordingly within the loop.

