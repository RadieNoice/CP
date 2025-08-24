# 342. Power of Four

**Link:** https://leetcode.com/problems/power-of-four/submissions/1746867393/

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

TAGS: Logic Error, Conditional Logic

1. **Key Issues**: Attempts 1-5 contain incomplete or incorrect conditional logic for checking if `log(n)/log(4)` is an integer.  Attempt 6 corrects the return value for n=0 but lacks a final return statement for the conditional check.  `isInteger` is also undefined.


2. **Evolution**: The coder attempted to use logarithms to identify powers of four.  The attempts gradually refined the conditional check, but failed to complete it or handle edge cases (n=0) correctly until the final attempt.  The commented-out code suggests exploration of other approaches that were not pursued.

