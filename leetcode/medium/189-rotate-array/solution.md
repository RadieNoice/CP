# 189. Rotate Array

**Link:** https://leetcode.com/problems/rotate-array/submissions/1755621621/

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
