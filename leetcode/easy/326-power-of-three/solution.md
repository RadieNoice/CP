# 326. Power of Three

**Link:** https://leetcode.com/problems/power-of-three/submissions/1734126803/

Given an integer n, return true if it is a power of three. Otherwise, return false. An integer n is a power of three, if there exists an integer x such that n == 3x.

```cpp
class Solution {
public:
    bool isPowerOfThree(int n) {
        if(n<=0)
        return false;
        while(n%3==0)
        n/=3;
        return n== 1;
    }
};
```

## Mistake Analysis

TAGS: Logic Error, Conditional Logic, Algorithm Choice

1. **Key Issues**: Attempts 1-3 incorrectly checked only divisibility by 3. Attempts 4-34 used `log` incorrectly, failing to handle floating-point precision. Attempts 35-41 had various logical errors and incomplete code. Attempt 42 finally correctly implemented iterative division.

2. **Evolution**: Initial attempts focused on flawed divisibility checks.  Later attempts used a logarithmic approach which was poorly implemented,  eventually moving towards a more efficient iterative solution in the final attempt.

