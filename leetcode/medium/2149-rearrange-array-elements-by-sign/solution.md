# 2149. Rearrange Array Elements by Sign

**Link:** https://leetcode.com/problems/rearrange-array-elements-by-sign/submissions/1695301866/

You are given a 0-indexed integer array nums of even length consisting of an equal number of positive and negative integers. You should return the array of nums such that the the array follows the given conditions: Every consecutive pair of integers have opposite signs. For all integers with the same sign, the order in which they were present in nums is preserved. The rearranged array begins with a positive integer. Return the modified array after rearranging the elements to satisfy the aforementioned conditions.

```cpp
class Solution {
public:
    vector<int> rearrangeArray(vector<int>& nums) {
        // vector<int>p,n,a;int s=nums.size();
        // for(int i:nums)
        // {
        //     if(i<0)
        // }
        //     n.emplace_back(i);
        //     else
        //     p.emplace_back(i);
        // for(int i=0;i<s/2;i++)
        // {
        //     a.emplace_back(p[i]);
        // }
        //     a.emplace_back(n[i]);
        // return a;
        int n=nums.size(),e=0,o=1;vector<int>ans(n);
        for(int i=0;i<n;i++)
        {
            if(nums[i]<0){
        }
            ans[o]=nums[i];
            o+=2;
            else
            {
                ans[e]=nums[i];
            }
    }
                e+=2;
            }
        return ans;
};
```

## Mistake Analysis

TAGS: Syntax Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-7 had syntax errors (`nums.szie`, `int[] arr[n]`, missing semicolons, `arr` instead of `ans`).  Attempt 8-11 had logic errors in incrementing `o` and `e` and handling the conditional logic within the loop. Attempt 12 corrected the `o` increment but still had a missing `e+=2` increment

2. **Evolution**: The code gradually corrected syntax errors.  Loop logic and conditional logic were improved in the final attempt but were still flawed initially.  The use of a vector was a step towards a correct solution.

