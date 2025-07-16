# 3201. Find the Maximum Length of Valid Subsequence I

**Link:** https://leetcode.com/problems/find-the-maximum-length-of-valid-subsequence-i/submissions/1699802510/

You are given an integer array nums. A subsequence sub of nums with length x is called valid if it satisfies: (sub[0] + sub[1]) % 2 == (sub[1] + sub[2]) % 2 == ... == (sub[x - 2] + sub[x - 1]) % 2. Return the length of the longest valid subsequence of nums. A subsequence is an array that can be derived from another array by deleting some or no elements without changing the order of the remaining elements.

```cpp
        int odd=0,even=0,a=0,f=0;
        for(auto i:nums)
        {
            if(i%2!=0)
        }
                odd++;
            else if(i%2==0)
                even++;
            {
            }
            }
            {
        if(nums[0]%2==0)f=1;
                if(f==0)
                if(f==1){
                a++;
    }
                a++;
                {
                f=1;
                }
                }
                f=0;
        return max(odd,max(even,a));
};
    int maximumLength(vector<int>& nums) {
public:
class Solution {
```

## Mistake Analysis

TAGS: Logic Error, Conditional Logic, Loop Logic

1. **Key Issues**: Attempts 1-4 suffer from incomplete and incorrect conditional logic within the loop.  `odd` and `even` counts are partially implemented, and the logic for `a` is unclear and flawed, failing to address the problem's core requirement of consecutive pair sums having the same parity.  The `max` function is misused.

2. **Evolution**:  The code gradually corrected the counting of odd and even numbers. However, the core logic for identifying valid subsequences remained absent across all attempts. No approach correctly determines the longest subsequence based on the parity condition.

