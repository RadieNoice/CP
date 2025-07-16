# 3201. Find the Maximum Length of Valid Subsequence I

**Link:** https://leetcode.com/problems/find-the-maximum-length-of-valid-subsequence-i/submissions/1699806434/

You are given an integer array nums. A subsequence sub of nums with length x is called valid if it satisfies: (sub[0] + sub[1]) % 2 == (sub[1] + sub[2]) % 2 == ... == (sub[x - 2] + sub[x - 1]) % 2. Return the length of the longest valid subsequence of nums. A subsequence is an array that can be derived from another array by deleting some or no elements without changing the order of the remaining elements.

```cpp
class Solution {
public:
    int maximumLength(vector<int>& nums) {
        int odd=0,even=0,a=0,f=0;
        if(nums[0]%2==0)f=1;
        for(auto i:nums)
        {
            if(i%2!=0)
            {
                odd++;
                if(f==0)
                {
                a++;
                f=1;
                }
            }
            else if(i%2==0)
            {
                even++;
                if(f==1){
                a++;
                f=0;
                }
            }
        }
        return max({odd,even,a});
    }
};
```

## Mistake Analysis

TAGS: Logic Error, Syntax Error, Conditional Logic

1. **Key Issues**: Attempt 1 has numerous syntax errors (missing semicolons, misplaced braces).  The core logic is flawed; it doesn't correctly track consecutive pairs with equal parity sums, and the conditional logic for `f` is unclear and ineffective.  The `max` function is used inappropriately.

2. **Evolution**: No evolution is shown as only one incomplete and incorrect attempt is provided.

