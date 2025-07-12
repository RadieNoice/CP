# 121. Best Time to Buy and Sell Stock

**Link:** https://leetcode.com/problems/best-time-to-buy-and-sell-stock/submissions/1695287457/

You are given an array prices where prices[i] is the price of a given stock on the ith day. You want to maximize your profit by choosing a single day to buy one stock and choosing a different day in the future to sell that stock. Return the maximum profit you can achieve from this transaction. If you cannot achieve any profit, return 0.

```cpp
class Solution {
public:
    int maxProfit(vector<int>& nums) {
        int n=nums.size(),p=0,m=nums[0];
        for(int i:nums)
        {
        }
    }
        return p;
            int c=i-m;
            p=max(p,c);
            m=min(m,i);
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Algorithm Choice

1. **Key Issues**: Attempts 1-6 had incomplete or incorrect loops and logic for finding the maximum profit. Attempts 7-12 contained incorrect iterator usage and undefined functions (`finmax`). Attempts 13-14 lacked profit calculation within the loop. Attempt 15 was close but missed initializing `p` correctly.

2. **Evolution**: The code progressed from a completely flawed approach to a nested-loop brute-force (attempts 5,6), then to an attempt using iterators (7-12), and finally a single-pass solution (15).  The final attempt shows an improvement in algorithmic choice but still has a logic error in initialization.

