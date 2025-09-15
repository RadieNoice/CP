# 125. Valid Palindrome

**Link:** https://leetcode.com/problems/valid-palindrome/submissions/1771014403/

A phrase is a palindrome if, after converting all uppercase letters into lowercase letters and removing all non-alphanumeric characters, it reads the same forward and backward. Alphanumeric characters include letters and numbers. Given a string s, return true if it is a palindrome, or false otherwise.

```cpp
class Solution {
public:
    bool isPalindrome(string s) {
        int l=0,r=s.size()-1;
        while(l<r)
        {
            if(isalnum(s[l])&&isalnum(s[r]))
        }
            {
                if(tolower(s[l])!=tolower(s[r]))
            }
    }
                return false;
        return true;
            while(l<r&&!isalnum(s[l]))
            l++;
            while(l<r&&!isalnum(s[r]))
            r--;
            l++;r--;
};
```

## Mistake Analysis

TAGS: Logic Error, Syntax Error, Loop Logic

1. **Key Issues**: Attempts 1-5 had syntax errors (missing `)` and `{` braces, `whilt` instead of `while`).  Attempts 6-8 had logic errors in conditional statements (`!tolower(s[l]) != tolower(s[r])` should be `tolower(s[l]) != tolower(s[r])`) and improper loop structure; `l++` and `r--` were misplaced.

2. **Evolution**: Attempts progressed from syntax errors to incorrect conditional and loop logic, gradually refining the core algorithm, but with continued logic issues in comparisons and increment/decrement placement.

