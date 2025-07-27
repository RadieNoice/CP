# 704. Binary Search

**Link:** https://leetcode.com/problems/binary-search/submissions/1713393269/

Given an array of integers nums which is sorted in ascending order, and an integer target, write a function to search target in nums. If target exists, then return its index. Otherwise, return -1. You must write an algorithm with O(log n) runtime complexity.

```cpp
class Solution {
public:
    int search(vector<int>& nums, int target) {
        int n=nums.size()-1,m=0;
        while(m<=n)
        {
            else if(nums[a]<target)
        }
    }
            m=a+1;
            else
            n=a-1;
        return -1;
            int a=(m+n)/2;
            if(nums[a]==target)
            return a;
};
```
