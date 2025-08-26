# 3000. Maximum Area of Longest Diagonal Rectangle

**Link:** https://leetcode.com/problems/maximum-area-of-longest-diagonal-rectangle/submissions/1748726148/

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
