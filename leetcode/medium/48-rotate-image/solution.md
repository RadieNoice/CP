# 48. Rotate Image

**Link:** https://leetcode.com/problems/rotate-image/submissions/1760183453/

You are given an n x n 2D matrix representing an image, rotate the image by 90 degrees (clockwise). You have to rotate the image in-place, which means you have to modify the input 2D matrix directly. DO NOT allocate another 2D matrix and do the rotation.

```cpp

        
        // int n=matrix.size();
        // for(int i=0;i<n;i++)
        // {
        //     for(int j=i+1;j<n;j++)
        //     {
        //         swap(matrix[i][j],matrix[j][i]);
        //     }
        // }
        // for(auto&i :matrix)
        // {
        //     reverse(i.begin(),i.end());
        // }
        for(int i=0;i<n;i++)
        {
                swap(matrix[i][j],matrix[j][i]);
        }
    }
            for(int j=i+1;j<n;j++){
            }
        for(auto&i: matrix)
        reverse(i.begin(),i.end());
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Syntax Error

1. **Key Issues**: Attempt 1 has multiple syntax errors due to misplaced and unclosed loops. The core logic for transposing and reversing is incomplete and incorrectly implemented.  `swap(matrix[i][j],matrix[j][i]);` is outside its needed loop.

2. **Evolution**: No evolution is shown as only one incomplete attempt is provided.  The commented-out code hints at a better approach (transpose then reverse rows), but it's not correctly implemented.

