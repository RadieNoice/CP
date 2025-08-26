# 3000. Maximum Area of Longest Diagonal Rectangle

**Link:** https://leetcode.com/problems/maximum-area-of-longest-diagonal-rectangle/submissions/1748729023/

You are given a 2D 0-indexed integer array dimensions. For all indices i, 0 <= i < dimensions.length, dimensions[i][0] represents the length and dimensions[i][1] represents the width of the rectangle i. Return the area of the rectangle having the longest diagonal. If there are multiple rectangles with the longest diagonal, return the area of the rectangle having the maximum area.

```cpp
class Solution {
public:
    int areaOfMaxDiagonal(vector<vector<int>>& num) {
        int  area;
        double diag=-1;
        for(auto& i:num)
        {
            double x=sqrt(i[0]*i[0]+i[1]*i[1]);
            //cout <<x<<" "<<i[0]<<" "<<i[1]<<endl;
            if(diag<x)
            {
                diag=x;area=i[0]*i[1];
            }
            else if (diag==x)
            area=max(area,i[0]*i[1]);
        }
        return area;
    }
};
```

## Mistake Analysis

TAGS: Logic Error, Conditional Logic

1. **Key Issues**: Attempt 1 incorrectly handles ties in diagonal length. It only considers the area of the first rectangle encountered with the maximum diagonal, not the maximum area among rectangles with the maximum diagonal.  The `else if` condition is flawed.

2. **Evolution**: No subsequent attempts were provided to analyze improvement.

