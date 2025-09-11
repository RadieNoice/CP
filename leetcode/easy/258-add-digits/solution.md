# 258. Add Digits

**Link:** https://leetcode.com/problems/add-digits/submissions/1767014669/

Given an integer num, repeatedly add all its digits until the result has only one digit, and return it.

```cpp
class Solution {
public:
    int addDigits(int num) {
        int x=0;
            while(num!=0)
            {
                x+=num%10;
            }
        while(true){
        }
                num=num/10;
        return x;
           // cout<<x<<endl;
            if(x>=10)
            {
            }
    }
                num=x;
                x=0;  
            else break;
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: All attempts suffered from improper loop control and conditional logic.  The `do-while` loops were incorrectly structured and didn't update `x` properly. The intended logic to repeatedly sum digits until a single digit remained was not implemented correctly.  The final `if` statements were useless.

2. **Evolution**: Attempts gradually corrected the `while` loop condition for summing digits.  However, the core flaw in handling the iterative summation and conditional logic remained unresolved until the final attempts.  The final attempts are still flawed.

