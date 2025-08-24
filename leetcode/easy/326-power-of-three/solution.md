# 326. Power of Three

**Link:** https://leetcode.com/problems/power-of-three/submissions/1746870573/

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

TAGS: Logic Error, Conditional Logic, Edge Cases

1. **Key Issues**: Attempt 1 is missing the main function body for `isPowerOfThree`. Both attempts use floating-point arithmetic (`log`) which can be inaccurate for large integers, leading to incorrect results for edge cases.  Neither properly handles the case of n=0.

2. **Evolution**: Attempt 2 added a check for `n==0`, but the fundamental floating-point precision issue remains unresolved.  The commented-out code suggests a potentially more robust iterative approach (not implemented).

