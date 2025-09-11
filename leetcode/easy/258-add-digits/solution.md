# 258. Add Digits

**Link:** https://leetcode.com/problems/add-digits/description/

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
