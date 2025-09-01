# 189. Rotate Array

**Link:** https://leetcode.com/problems/rotate-array/submissions/1755616999/

Given an integer array nums, rotate the array to the right by k steps, where k is non-negative.

```cpp
#include <algorithm>
class Solution {
public:
    void rotate(vector<int>& nums, int k) {
        int n=nums.size();
        k%=n;
        if(n>1&&k>0){
        reverse(nums.begin(),nums.begin()+n-k);
        reverse(nums.begin()+n-k,nums.end());
        reverse(nums.begin(),nums.end());
        // nums.insert(nums.end(),nums.begin(),nums.begin()+n-k);
        // nums.erase(nums.begin(),nums.begin()+n-k);
        }
    }
};
```

## Mistake Analysis

TAGS: Algorithm Choice, Logic Error, Array Bounds

1. **Key Issues**: Attempt 1 uses three reversals to rotate. While correct, it's unnecessarily complex and prone to off-by-one errors in the reversal ranges if `k` is near `n`.  The commented-out code suggests an initially flawed approach using `insert` and `erase`, which is inefficient.

2. **Evolution**: No further attempts are provided for analysis.  A more efficient approach would involve a single pass using a circular buffer or temporary array.

