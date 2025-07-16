# 3201. Find the Maximum Length of Valid Subsequence I

**Link:** https://leetcode.com/problems/find-the-maximum-length-of-valid-subsequence-i/submissions/

You are given an integer array nums. A subsequence sub of nums with length x is called valid if it satisfies: (sub[0] + sub[1]) % 2 == (sub[1] + sub[2]) % 2 == ... == (sub[x - 2] + sub[x - 1]) % 2. Return the length of the longest valid subsequence of nums. A subsequence is an array that can be derived from another array by deleting some or no elements without changing the order of the remaining elements.

```cpp
class Solution {
public:
    int maximumLength(vector<int>& nums) {
        int odd=0,even=0,a=0,f=0;
        if(nums[0]%2==0)f=1;
        for(auto i:nums)
        {
            int c=i%2;
            if(c!=0)
            {
                odd++;
                if(!f)
                {
                a++;
                f=1;
                }
            }
            else if(c==0)
            {
                even++;
                if(f){
                a++;
                f=0;
                }
            }
        }
        return max({odd,even,a});
    }
```
