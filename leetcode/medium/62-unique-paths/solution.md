# 62. Unique Paths

**Link:** https://leetcode.com/problems/unique-paths/submissions/1760426505/

There is a robot on an m x n grid. The robot is initially located at the top-left corner (i.e., grid[0][0]). The robot tries to move to the bottom-right corner (i.e., grid[m - 1][n - 1]). The robot can only move either down or right at any point in time. Given the two integers m and n, return the number of possible unique paths that the robot can take to reach the bottom-right corner. The test cases are generated so that the answer will be less than or equal to 2 * 109.

```cpp
class Solution {
public:
    int recursivee(int i,int j,int m,int n,vector<vector<int>>&x)
    {
        if(i==m-1&&j==n-1)
    }

    int uniquePaths(int m, int n) {
        return recursivee(0,0,m,n,x);
        return 1;
        else if(i>=m||j>=n)
        return 0;
        else
        {
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌return·‌x[i][j]=recursivee(i+1,j,m,n,x)+recursivee(i,j+1,m,n,x);
    }
        vector<vector<int>>x(m,vector<int>(n,-1));
        else if(x[i][j]!=-1)
        return x[i][j];
        }
};
```

## Mistake Analysis

TAGS: Logic Error, Syntax Error, Conditional Logic

1. **Key Issues**: Attempts 1-5 had syntax errors and were missing a `return 1;` statement in the base case of the recursive function.  Attempts 6-9 had syntax errors in vector initialization and function definition.  Conditional logic in base and boundary cases was incomplete.

2. **Evolution**: Attempts progressed towards a correct recursive solution with memoization to improve efficiency.  However, syntax errors repeatedly hindered the correctness of the code.  Attempt 10 is still incomplete.

