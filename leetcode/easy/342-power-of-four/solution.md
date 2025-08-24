# 342. Power of Four

**Link:** https://leetcode.com/problems/power-of-four/submissions/1746857558/

Given an integer n, return true if it is a power of four. Otherwise, return false. An integer n is a power of four, if there exists an integer x such that n == 4x.

```cpp
    bool isPowerOfFour(int n) {
        if(n<=0)
        for(int i=0;i<s.size();i++)
        {
            if(t==0&&s[i]=='1')
            t++;
            else if(t==1&&s[i]=='1')
            return false;
        return true;
        
    }
        if(n==2)
        return false;
class Solution {
public:
        }
        string s=bitset<32>(n).to_string();
        int t=0;
        return false;
        reverse(s.begin(),s.end());
        cout<<s<<endl;
        cout<<s;
        if(t==0)
        return false;
            if(s[i]=='1'&(i+1)%2==0)
            return false;
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-7 had incomplete loops and incorrect conditional logic for checking the single '1' bit in the binary representation. Attempts 8-43 were largely syntactically incorrect with missing braces and erroneous `reverse()` calls.  The core logic of checking only one '1' bit and its position was never fully implemented correctly.

2. **Evolution**: Initial attempts focused on a flawed binary bit-counting approach. Later attempts tried to address this by reversing the bitset string, but syntax and logic errors prevented a functional solution. The core problem of correctly identifying and validating the single '1' bit was never fixed.

