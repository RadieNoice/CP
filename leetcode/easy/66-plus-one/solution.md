# 66. Plus One

**Link:** https://leetcode.com/problems/plus-one/submissions/1760748725/

You are given a large integer represented as an integer array digits, where each digits[i] is the ith digit of the integer. The digits are ordered from most significant to least significant in left-to-right order. The large integer does not contain any leading 0's. Increment the large integer by one and return the resulting array of digits.

```cpp
class Solution {
public:
    vector<int> plusOne(vector<int>& digits) {
        int n=digits.size(),r=0,i=n-1;
        do
        {
            if(digits[i]+1>9)
        }while(r==1&&i>=0);
        return digits;
            {
                digits[i]=(digits[i]+1)%10;
            }
    }
                r=1;
                i--;
            else
        if(r==1)
        digits.insert(digits.begin(),1);
            { digits[i]+=1;
            }
                r=0;
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-5 had misplaced or missing code blocks, resulting in incorrect increment logic. The `do-while` loop was improperly structured, not correctly updating `r` or handling carry-over. Attempt 6 added a leading 1 correctly but lacked proper code structure. Attempt 7 still suffered from improperly structured conditional and loop logic.


2. **Evolution**: Attempts progressed towards a correct `do-while` loop structure and carry handling.  The addition of a leading '1' (Attempt 6) addressed the edge case of a number with all 9s.  However, the code blocks and conditional statements were inconsistently structured, hindering correct compilation and execution until the final attempt.

