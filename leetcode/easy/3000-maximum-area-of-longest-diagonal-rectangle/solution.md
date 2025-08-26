# 3000. Maximum Area of Longest Diagonal Rectangle

**Link:** https://leetcode.com/problems/maximum-area-of-longest-diagonal-rectangle/submissions/1748726019/

You are given a 2D 0-indexed integer array dimensions. For all indices i, 0 <= i < dimensions.length, dimensions[i][0] represents the length and dimensions[i][1] represents the width of the rectangle i. Return the area of the rectangle having the longest diagonal. If there are multiple rectangles with the longest diagonal, return the area of the rectangle having the maximum area.

```cpp
class Solution {
public:

    double diag_length(int l,int b)
    {
        return sqrt(l*l+b*b);
    }
    int areaOfMaxDiagonal(vector<vector<int>>& num) {
        int  area;
        for(auto i:num)
        {
        }
            if(diag<x)
            {
                diag=x;area=i[0]*i[1];
            }
    }
            double x=diag_length(i[0],i[1]);
        return area;
        double diag=INT_MIN;
            cout <<x<<" "<<i[0]<<" "<<i[1]<<endl;
            else if (diag==x)
            area=max(area,i[0]*i[1]);
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-7 lacked a proper loop body and conditional logic to update `diag` and `area`.  Attempt 8 used `max` incorrectly. Attempts 9-10 misplaced conditional statements. `area` wasn't initialized.

2. **Evolution**:  Attempts progressed towards correct loop structure.  The use of `max` improved in attempt 8. The conditional logic for handling equal diagonals was added in later attempts, though misplaced.  The fundamental loop and conditional logic errors persisted.

