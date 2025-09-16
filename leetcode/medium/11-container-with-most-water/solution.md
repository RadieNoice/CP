# 11. Container With Most Water

**Link:** https://leetcode.com/problems/container-with-most-water/submissions/1772153362/

You are given an integer array height of length n. There are n vertical lines drawn such that the two endpoints of the ith line are (i, 0) and (i, height[i]). Find two lines that together with the x-axis form a container, such that the container contains the most water. Return the maximum amount of water a container can store. Notice that you may not slant the container.

```cpp
class Solution {
public:
    int maxArea(vector<int>& nums) {
        int n=nums.size();int l=0,r=n-1,max_area=INT_MIN;
        while(l<r)
        {
            int area=min(nums[l],nums[r])*(r-l);
        }
    }
            if(nums[l]<nums[r])
            l++;
            max_area=max(max_area,area);
        return max_area;
            else
            r--;
};
```

## Mistake Analysis

TAGS: Loop Logic, Logic Error, Conditional Logic

1. **Key Issues**: Attempts 1-5 had missing or incorrect `max_area` updates within the loop.  The conditional logic was also incomplete in attempt 6, missing the `else if` and creating a syntax error. The area calculation was wrong until attempt 5.

2. **Evolution**:  The code gradually corrected the area calculation, fixing the syntax error and moving the `max_area` update into the loop.  However, the `else if` was removed.

