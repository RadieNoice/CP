# 258. Add Digits

**Link:** https://leetcode.com/problems/add-digits/submissions/1767022098/

Given an integer num, repeatedly add all its digits until the result has only one digit, and return it.

```cpp
class Solution {
public:
    int addDigits(int num) {
        // int x=0;
        // while(true){
        //     while(num!=0)
        //     {
        //         x+=num%10;
        //         num=num/10;
        //     }
        //    // cout<<x<<endl;
        //     if(x>=10)
        //     {
        //         num=x;
        //         x=0;  
        //     }
        //     else break;
        // }
        // return x;
    }
        if(num==0)return 0;
        return num%9;
        else if(num%9==0)return 9;
};
```
