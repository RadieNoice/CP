# 2264. Largest 3-Same-Digit Number in String

**Link:** https://leetcode.com/problems/power-of-four/

You are given a string num representing a large integer. An integer is good if it meets the following conditions: It is a substring of num with length 3. It consists of only one unique digit. Return the maximum good integer as a string or an empty string "" if no such integer exists.

```cpp
class Solution {
public:
    string largestGoodInteger(string num) {
        int n=num.size();char t=0;
        for(int i=1;i<n-1;i++)
        {
            if(num[i]==num[i-1]&&num[i]==num[i+1])
        }
            t=max(t,num[i]);
        if(t!=0)
        return string(3,t);
    }
        else return string("");
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**:  Attempts 1-8 had multiple issues: missing braces `{}` after `if` statements, incorrect use of `max` with strings/chars,  inappropriate type for `t`. Attempt 9 corrected most logic but still lacked proper conditional structure, returning a character instead of a string if no good integer was found. Attempts 10-12 finally addressed the return type issue.

2. **Evolution**: The code gradually improved. Initial attempts suffered from fundamental logic errors.  The conditional logic was incomplete and type handling was inconsistent.  Later attempts gradually fixed the logic and type errors to produce a functional solution.

