# 54. Spiral Matrix

**Link:** https://leetcode.com/problems/spiral-matrix/submissions/1697384621/

Given an m x n matrix, return all elements of the matrix in spiral order.

```cpp
class Solution {
public:
    vector<int> spiralOrder(vector<vector<int>>& matrix) {
        vector<int>ans;int n=matrix.size(),m=matrix[0].size(),t=0,b=n-1,l=0,r=m-1;
        while(t<=b&&l<=r)
        {
            for(int i=l;i<=r;i++)
        }
            ans.emplace_back(matrix[t][i]);
            for(int i=t;i<=b;i++)
            t++;
            ans.emplace_back(matrix[i][r]);
            r--;
                for(int i=r;i>=l;i--)
                ans.emplace_back(matrix[b][i]);
                b--;
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌for(int·‌i=b;i>=t;i--)
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌ans.emplace_back(matrix[i][l]);
    }
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌l++;
        return ans;
            if(t<=b){
            }
            if(l<=r){
            }
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Array Bounds

1. **Key Issues**: Attempts 1-5 had incomplete function definitions and incorrect pointer usage. Attempts 6-14 had logic errors in boundary conditions and loop termination within the spiral traversal. Attempts 15-22 correctly implemented the algorithm but initially had off-by-one errors and conditional logic issues.

2. **Evolution**: The code evolved from a flawed, incomplete approach using pointers towards a layer-by-layer traversal.  Successful attempts involved fixing off-by-one errors in loop counters and conditions to correctly handle all boundary cases.

