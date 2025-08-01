# 118. Pascal's Triangle

**Link:** https://leetcode.com/problems/pascals-triangle/

Given an integer numRows, return the first numRows of Pascal's triangle. In Pascal's triangle, each number is the sum of the two numbers directly above it as shown:

```cpp
        if(n>=1)
        triangle.push_back({1});
        if(n>=2)
        triangle.push_back({1,1});
        if(n>2)
        {
            int s=3;
            while(triangle.size()<n)
            {
                vector<int>x(s);
                x[0]=1;
                x[s-1]=1;
        vector<vector<int>>triangle;
                for(int i=1;i<s-1;i++)
                {
                    x[i]=triangle[s-2][i]+triangle[s-2][i-1];
                }
                s++;
                triangle.push_back(x);
            }
        }
        return triangle;
    }
};
```

## Mistake Analysis

TAGS: Logic Error, Array Bounds, Loop Logic

1. **Key Issues**: Attempt 1 is mostly commented out. The uncommented part returns an empty vector. The commented code has a logic error in calculating elements; it attempts to access `triangle[s-2]` before those elements exist.  `x` vector's size is incorrect, leading to array bounds issues in the loop.  The loop logic for constructing rows is flawed.

2. **Evolution**: No evolution is shown as only one incomplete, incorrect attempt is provided.

