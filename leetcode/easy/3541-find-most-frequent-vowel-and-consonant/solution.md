# 3541. Find Most Frequent Vowel and Consonant

**Link:** https://leetcode.com/problems/find-most-frequent-vowel-and-consonant/submissions/1769095010/

You are given a string s consisting of lowercase English letters ('a' to 'z'). Your task is to: Find the vowel (one of 'a', 'e', 'i', 'o', or 'u') with the maximum frequency. Find the consonant (all other letters excluding vowels) with the maximum frequency. Return the sum of the two frequencies.

```cpp
class Solution {
public:
    int maxFreqSum(string s) {
        unordered_map<char,int>v,c;int mv=0,mc=0;
        for(auto&i:s)
        {
            if(i=='a'||i=='e'||i=='i'||i=='o'||i=='u'){
        }
            v[i]++;
            mv=max(mv,v[i]);
            }
            else
            {
                c[i]++;
            }
    }
                mc=max(mc,c[i]);
        return mv+mc;
};
```

## Mistake Analysis

TAGS: Syntax Error, Logic Error, Conditional Logic

1. **Key Issues**: Attempt 1-3 had syntax errors (`unorderd_map`, `mac`).  Attempt 4 corrected syntax but had a logic error: the `if` condition for vowels was empty,  never incrementing `v`.  The `else` block was also incorrectly indented.

2. **Evolution**: Attempts progressed by fixing syntax errors (`unordered_map`, `max`). However, the core logic error in the vowel counting remained until the last attempt.  Correct indentation is crucial for conditional logic.

