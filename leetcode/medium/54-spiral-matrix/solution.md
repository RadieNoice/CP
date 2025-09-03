# 54. Spiral Matrix

**Link:** https://leetcode.com/problems/spiral-matrix/description/

Given an m x n matrix, return all elements of the matrix in spiral order.

```cpp

    //     vector<int>ans;int n=matrix.size(),m=matrix[0].size(),t=0,b=n-1,l=0,r=m-1;
    //     while(t<=b&&l<=r)
    //     {
    //         for(int i=l;i<=r;i++)
    //         ans.emplace_back(matrix[t][i]);
        return ans;
    //         t++;
    //         for(int i=t;i<=b;i++)
    //         ans.emplace_back(matrix[i][r]);
    //         r--;
    //         if(t<=b){
        }
            l++;}
                ans.emplace_back(matrix[i][l]);
            for(int i=b;i>=t;i--)
            if(l<=r){
                b--;}
                ans.emplace_back(matrix[b][i]);
            for(int i=r;i>=l;i--)
            if(t<=b){
                r--;
                ans.emplace_back(matrix[i][r]);
    //             for(int i=r;i>=l;i--)
    //             ans.emplace_back(matrix[b][i]);
    //             b--;
    //         }
    //         if(l<=r){
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**:  Attempts 1-8 are missing the core `while` loop and proper conditional logic to control the spiral traversal.  Loops are incomplete or incorrectly nested, leading to incorrect element order or omissions.  Attempts 9-11 lack the core logic, only showing commented-out correct code.

2. **Evolution**: The commented code in later attempts suggests understanding of the correct algorithm (using a `while` loop and four nested `for` loops). However, none of the attempts successfully implemented it.  The initial attempts lacked the fundamental structure for the solution.

