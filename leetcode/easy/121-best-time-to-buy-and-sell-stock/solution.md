# 121. Best Time to Buy and Sell Stock

**Link:** https://leetcode.com/problems/best-time-to-buy-and-sell-stock/description/

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
