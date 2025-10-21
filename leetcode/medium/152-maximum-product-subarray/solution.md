# 152. Maximum Product Subarray

**Link:** https://leetcode.com/problems/maximum-product-subarray/submissions/1807200736/

Given an integer array nums, find a subarray that has the largest product, and return the product. The test cases are generated so that the answer will fit in a 32-bit integer. Note that the product of an array with a single element is the value of that element.

```cpp
class Solution {
public:
    int maxProduct(vector<int>& nums) {
        int x=nums[0],y=x,ans=x;
        for(int i=1;i<nums.size();i++)
        {
            x=max({x*nums[i],y*nums[i],nums[i]});
        }
    }
            y=min({z*nums[i],y*nums[i],nums[i]});
            ans=max(x,ans);
            int z=x;
        return ans;
};
```
