# 189. Rotate Array

**Link:** https://leetcode.com/problems/rotate-array/submissions/1755621278/

Given an integer array nums, rotate the array to the right by k steps, where k is non-negative.

```cpp
#include <algorithm>
class Solution {
public:
    void rotate(vector<int>& nums, int k) {
        // int n=nums.size();
        // k%=n;
        // if(n>1&&k>0){
        // reverse(nums.begin(),nums.begin()+n-k);
        // reverse(nums.begin()+n-k,nums.end());
        // reverse(nums.begin(),nums.end());
        // // nums.insert(nums.end(),nums.begin(),nums.begin()+n-k);
        // // nums.erase(nums.begin(),nums.begin()+n-k);
        // }
    }

        int n=nums.size();
        reverse(nums.begin(),nums.begin()+n-k);
        reverse(nums.begin()+n-k,nums.end());
        reverse(nums.begin(),nums.end());
        k%=n;//when k > n in that case we need k as k%n
        if(n>1&&k>0){
        }
};
```

## Mistake Analysis

TAGS: Logic Error, Algorithm Choice, Edge Cases

1. **Key Issues**: Attempt 1 and 2 both have the same core issue. The `k %= n;` line to handle k > n is placed incorrectly outside the `rotate` function in both attempts and the commented-out code suggests a misunderstanding of the 3-reverse algorithm.


2. **Evolution**: No significant evolution in logic. Attempt 2 simply moved the `k %= n` line but failed to integrate it correctly.  The fundamental algorithm was flawed, not improved.

