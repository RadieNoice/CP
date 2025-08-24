# 342. Power of Four

**Link:** https://leetcode.com/problems/power-of-four/submissions/1746868158/

Given an integer n, return true if it is a power of four. Otherwise, return false. An integer n is a power of four, if there exists an integer x such that n == 4x.

```cpp
        // if(n==2)
        // return false;
        // if(n<=0)
        // return false;
        // string s=bitset<32>(n).to_string();
        // int t=0;
        // cout<<s<<endl;
        // reverse(s.begin(),s.end());
        // cout<<s;
        // for(int i=0;i<s.size();i++)
        // {
        //     if(s[i]=='1'&(i+1)%2==0)
        //     return false;
        //     if(t==0&&s[i]=='1')
        //     t++;
        //     else if(t==1&&s[i]=='1')
        //     return false;
        // }
        // if(t==0)
        return true;
        return false;
        if(floor(x)==x)
    bool isPowerOfFour(int n) {
public:
class Solution {
        double x=log(n)/log(4);
        if(n==0)
        return false;
```

## Mistake Analysis

TAGS: Logic Error, Conditional Logic, Algorithm Choice

1. **Key Issues**: Attempt 1 uses an inefficient and incorrect bit manipulation approach (commented-out code).  The final `if` statement is incomplete and has syntax errors. It attempts to use logarithms, but lacks proper checks for `n` being 0 or negative.

2. **Evolution**: No significant improvement between attempts; Attempt 1 is fundamentally flawed.  A correct solution would efficiently check for divisibility by 4 repeatedly, or use bit manipulation to check for a single set bit and its position.

