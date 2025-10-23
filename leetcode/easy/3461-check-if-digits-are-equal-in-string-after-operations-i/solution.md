# 3461. Check If Digits Are Equal in String After Operations I

**Link:** https://leetcode.com/problems/check-if-digits-are-equal-in-string-after-operations-i/submissions/1809064299/

You are given a string s consisting of digits. Perform the following operation repeatedly until the string has exactly two digits: For each pair of consecutive digits in s, starting from the first digit, calculate a new digit as the sum of the two digits modulo 10. Replace s with the sequence of newly calculated digits, maintaining the order in which they are computed. Return true if the final two digits in s are the same; otherwise, return false.

```cpp
class Solution {
public:
    bool hasSameDigits(string s) {
        while (s.length()!=2)
        {
            string x="";
            for(int i=0;i<s.length()-1;i++)
        }
            {
            }
    }
                x+=(s[i]+s[i+1])%10;
            s=x;
        if(s[0]==s[1])
        return true;
        return false;
                
                

};
```
