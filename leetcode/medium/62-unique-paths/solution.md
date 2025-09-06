# 62. Unique Paths

**Link:** https://leetcode.com/problems/unique-paths/submissions/1761223010/

There is a robot on an m x n grid. The robot is initially located at the top-left corner (i.e., grid[0][0]). The robot tries to move to the bottom-right corner (i.e., grid[m - 1][n - 1]). The robot can only move either down or right at any point in time. Given the two integers m and n, return the number of possible unique paths that the robot can take to reach the bottom-right corner. The test cases are generated so that the answer will be less than or equal to 2 * 109.

```cpp
    //     return 0;
    //     else if(x[i][j]!=-1)
    //     return x[i][j];
    //     else
    //     {
    //         return x[i][j]=recursivee(i+1,j,m,n,x)+recursivee(i,j+1,m,n,x);
    //     }
    // }

    int uniquePaths(int m, int n) {
        // vector<vector<int>>x(m,vector<int>(n,-1));
        // return recursivee(0,0,m,n,x);
        int x=m+n-2,r=min(m-1,n-1);
        return round(ncr);
        for(int i=1;i<=r;i++)
        {
            ncr*=(double)x/i;
        }
            x--;

            //cout<<x<<" "<<i<<endl;
    }
        double ncr=1;
};
```

## Mistake Analysis

TAGS: Logic Error, Algorithm Choice, Off By One

1. **Key Issues**: Attempts 1-8 incorrectly calculated combinations using an iterative approach with flawed logic and off-by-one errors. Attempts 9-16 used a similar approach, but with type errors and inaccurate rounding.  Attempt 17 finally addressed type issues with `double` and `round()`.

2. **Evolution**: The code progressed from a flawed iterative combination calculation to a partially correct version using `double` for intermediate calculations and rounding for the final result, but the algorithm choice remains inefficient compared to dynamic programming.

