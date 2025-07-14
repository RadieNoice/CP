# 48. Rotate Image

**Link:** https://leetcode.com/problems/rotate-image/submissions/1697338362/

You are given an n x n 2D matrix representing an image, rotate the image by 90 degrees (clockwise). You have to rotate the image in-place, which means you have to modify the input 2D matrix directly. DO NOT allocate another 2D matrix and do the rotation.

```cpp
class Solution {
public:
    void rotate(vector<vector<int>>& matrix){
        int n=matrix.size();
        for(int i=0;i<n;i++)
        {
            for(int j=i+1;j<n;j++)
            {
                swap(matrix[i][j],matrix[j][i]);
            }
        }
        for(auto&i :matrix)
        {
            reverse(i.begin(),i.end());
        }
    }
};
```

## Mistake Analysis

TAGS: Algorithm Choice, Logic Error

1. **Key Issues**: Attempts 1-4 incorrectly used `sort` (Attempt 1-2)  or failed to use a reference to rows (Attempt 4) for reversing rows.  The correct algorithm involves transposing the matrix and then reversing each row.

2. **Evolution**:  The code evolved from an incorrect sorting approach (Attempts 1-2) to using `reverse` (Attempt 3). Attempt 5 finally corrected the reference issue in the loop.

