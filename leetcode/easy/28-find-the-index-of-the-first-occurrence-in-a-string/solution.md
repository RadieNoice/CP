# 28. Find the Index of the First Occurrence in a String

**Link:** https://leetcode.com/problems/find-the-index-of-the-first-occurrence-in-a-string/submissions/1778908571/

Given two strings needle and haystack, return the index of the first occurrence of needle in haystack, or -1 if needle is not part of haystack.

```cpp
class Solution {
public:
    int strStr(string ss, string needle) {
        int k=needle.size(),n=ss.size();
        for(int i=0;i<n;i++)
        {
        }
    }
            if(s==needle)
            return i;
        return -1;
            string s=ss.substr(i,k);
            //cout<<s<<endl;
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Algorithm Choice

1. **Key Issues**: Attempts 1-4 had numerous logic errors in their nested loops and conditional statements, failing to correctly compare substrings. Attempts 5-12 implemented a flawed algorithm with incorrect loop bounds and substring extraction; Attempt 13 finally corrected the loop bound but still lacked the `if(s==needle)` within the loop.


2. **Evolution**: The code evolved from a completely incorrect nested loop approach (Attempts 1-4) to a sliding window approach (Attempts 5-13).  Attempts gradually corrected the loop conditions and substring extraction, converging towards a correct solution in Attempt 13.  However, a crucial `if` statement checking string equality was missing until the final attempt.

