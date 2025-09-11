# 258. Add Digits

**Link:** https://leetcode.com/problems/add-digits/

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

TAGS: Logic Error, Loop Logic

1. **Key Issues**: All attempts suffer from fundamental logic errors in the loop structures and conditional statements for handling multi-digit sums.  Incorrect loop termination conditions and missing updates to `num` and `x` prevent proper iterative summing.

2. **Evolution**: Attempts gradually improved the while loop condition, moving closer to correctly accumulating digits.  However, none successfully implemented the iterative digit-summing and single-digit check required by the problem.  The `do-while` loop was consistently misused.

