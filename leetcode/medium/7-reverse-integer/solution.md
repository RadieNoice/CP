# 7. Reverse Integer

**Link:** https://leetcode.com/problems/reverse-integer/submissions/1778547615/

Given a signed 32-bit integer x, return x with its digits reversed. If reversing x causes the value to go outside the signed 32-bit integer range [-231, 231 - 1], then return 0. Assume the environment does not allow you to store 64-bit integers (signed or unsigned).

```cpp
class Solution {
public:
    int reverse(int x) {
        string s=to_string(x);int l=0,r=s.size()-1;long long num;
        if(s[0]=='-'||s[0]=='0')
        l=1;
        while(l<r)
        return num;
        {
            swap(s[l],s[r]);
        }
    }
            l++;r--;
        from_chars(s.data(), s.data() + s.size(), num);
        //cout<<s;
        if(num>pow(2,31)-1||num<-pow(2,31))
        return 0;
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Input Handling

1. **Key Issues**:  Attempts 1-5 had logic errors in the `while` loop, prematurely returning before reversing the string. Attempt 6 used `long long`, but the range check was incorrect.  `from_chars` was misused; string reversal wasn't completed inside the loop.

2. **Evolution**: Attempts gradually corrected the loop logic and attempted to handle the integer overflow by using a `long long` and checking the range, but the range check was flawed initially.  The main issue was improperly placed `return` statement in the `while` loop.

