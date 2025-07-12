# 73. Set Matrix Zeroes

**Link:** https://leetcode.com/problems/set-matrix-zeroes/submissions/1695538288/

Given an m x n integer matrix matrix, if an element is 0, set its entire row and column to 0's. You must do it in place.

```cpp
            for(int j=0;j<c;j++)
            {
            }
                if(matrix[i][j]==0)
                {
                }
                    z.emplace_back(i,j);
            for (int i=0;i<r;i++)
            {   
            }
            for (int i=0;i<c;i++)
            {
            }

    }
        {
public:
    void setZeroes(vector<vector<int>>& matrix) {
        int r=matrix.size(),c=matrix[0].size();
        for(int i=0;i<r;i++)
class Solution {
                matrix[j.first][i]=0;
                matrix[i][j.second]=0;
        vector<pair<int,int>>z;
        for(auto j:z){
        }
        }
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Array Bounds

1. **Key Issues**: Attempts 1-7 failed to correctly identify and process zero elements.  Incorrect array indexing (`matrix[r][c]`) caused array bounds issues.  Attempts 8-16 partially corrected zero identification but lacked complete row/column zeroing logic.  Incorrect loop usage and data structure application hindered progress.

2. **Evolution**: Attempts gradually corrected the zero identification (using `matrix[i][j]`). However, the attempts to set the rows and columns to zero failed until an appropriate data structure (`vector<pair<int,int>>`) was introduced to store the coordinates of zeroes. The final attempts still have unimplemented loop bodies for completing the row/column zeroing.

