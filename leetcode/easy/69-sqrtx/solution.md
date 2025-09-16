# 69. Sqrt(x)

**Link:** https://leetcode.com/problems/sqrtx/submissions/1772462835/

Given a non-negative integer x, return the square root of x rounded down to the nearest integer. The returned integer should be non-negative as well. You must not use any built-in exponent function or operator.

```java
class Solution {
    public int mySqrt(int x) {
        return (int)Math.sqrt(x);
    }
}
```

## Mistake Analysis

TAGS: Algorithm Choice, Logic Error

1. **Key Issues**: Both attempts directly used the built-in `sqrt()` function, violating the problem constraints.  Attempt 1 has a syntax error ( `Math.sqrt()` is Java, not C++).

2. **Evolution**: No improvement; both attempts failed to implement a suitable algorithm (e.g., binary search or Newton's method) to compute the square root without using the built-in function.

