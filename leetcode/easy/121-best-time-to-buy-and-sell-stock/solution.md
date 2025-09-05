# 121. Best Time to Buy and Sell Stock

**Link:** https://leetcode.com/problems/best-time-to-buy-and-sell-stock/

You are given an array prices where prices[i] is the price of a given stock on the ith day. You want to maximize your profit by choosing a single day to buy one stock and choosing a different day in the future to sell that stock. Return the maximum profit you can achieve from this transaction. If you cannot achieve any profit, return 0.

```cpp
class Solution {
public:
    int maxProfit(vector<int>& nums) {
        // int n=nums.size(),p=0,m=nums[0];
        // for(int i:nums)
        // {
        //     int c=i-m;
        //     p=max(p,c);
        //     m=min(m,i);
        // }
        // return p;


        int mp=0,s=nums[0];
        for(int&i:nums)
        {
            int p=i-s;
        }
    }
            mp=max(mp,p);
            s=min(i,s);
        return mp;
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Syntax Error

1. **Key Issues**: Attempt 1 has multiple syntax errors (missing closing brace and misplaced `mp=max(mp,p);` and `s=min(i,s);`). The core logic is flawed; the profit calculation (`p=i-s;`) is inside the loop but the `max` and `min` updates are outside the loop's scope, preventing correct profit tracking.

2. **Evolution**: No evolution is shown; only one incomplete attempt is provided.  The commented-out code suggests a potentially correct approach, but it is not implemented.

