# 35. Search Insert Position

**Link:** https://leetcode.com/problems/search-insert-position/submissions/1713529128/

Given a sorted array of distinct integers and a target value, return the index if the target is found. If not, return the index where it would be if it were inserted in order. You must write an algorithm with O(log n) runtime complexity.

```cpp
class Solution {
public:
    int searchInsert(vector<int>& nums, int target) {
       int m=0,n=nums.size()-1; 
       while(m<=n)
       {
            else if(nums[a]>target)
       }
    }
            int a=(m+n)/2;
            n=a-1;
            if(nums[a]==target)
            return a;
            else 
            m=a+1;
       return m;
};
```
