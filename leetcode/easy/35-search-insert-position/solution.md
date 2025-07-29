# 35. Search Insert Position

**Link:** https://leetcode.com/problems/search-insert-position/description/

Given a sorted array of distinct integers and a target value, return the index if the target is found. If not, return the index where it would be if it were inserted in order. You must write an algorithm with O(log n) runtime complexity.

```cpp
class Solution {
public:
    int searchInsert(vector<int>& nums, int target) {
       int m=0,n=nums.size()-1; 
       while(m<=n)
       {
            int a=(m+n)/2;
            if(nums[a]==target)
            return a;
            else if(nums[a]>target)
            n=a-1;
            else 
            m=a+1;
       }
       return m;
    }
};
```

## Mistake Analysis

TAGS: Algorithm Choice, Edge Cases, Conditional Logic

1. **Key Issues**: Attempt 1 uses binary search, but incorrectly handles the insertion point when the target is not found. The return value `m` might be off by one depending on the last comparison.  The algorithm doesn't explicitly address the case of an empty input array.


2. **Evolution**: No further attempts were provided to analyze.

