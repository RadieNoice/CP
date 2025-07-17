# 118. Pascal's Triangle

**Link:** https://leetcode.com/problems/pascals-triangle/submissions/1701462023/

Given an integer numRows, return the first numRows of Pascal's triangle. In Pascal's triangle, each number is the sum of the two numbers directly above it as shown:

```cpp
        if(n>2)
        {
        }

        if(n>=1)
        triangle.push_back({1});
        if(n>=2)
        triangle.push_back({1,1});
            int s=3;
            while(triangle.size()<n)
            {
                vector<int>x(s);
            }
                x[0]=1;
                x[s-1]=1;
                for(int i=1;i<s-1;i++)
                {
                    x[i]=triangle[s-2][i]+triangle[s-2][i-1];
                }
    }
                s++;
                triangle.push_back(x);
        return triangle;
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Array Bounds

1. **Key Issues**: Attempts 1-12 failed to correctly populate `x` within the while loop.  The `while` loop was missing the core logic for calculating Pascal's triangle values. `s` was incorrectly used for indexing. Array bounds were not checked.

2. **Evolution**: Attempts progressed towards correctly calculating `x` using `triangle[s-2]`, but still had logic errors in the `while` loop's body until Attempt 13.  Attempt 13 is closer to a correct solution, but would still need additional logic to handle initial conditions fully.

