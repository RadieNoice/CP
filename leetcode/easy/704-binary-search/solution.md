# 704. Binary Search

**Link:** https://leetcode.com/problems/binary-search/submissions/1713393139/

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

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-8 had incomplete conditional logic within the `while` loop, failing to update `n` in all cases. Attempts 9-21 lacked proper `a` variable initialization and incorrect loop conditions, leading to infinite loops or incorrect mid-point calculation.  The core binary search logic was never fully implemented correctly.

2. **Evolution**: Attempts showed gradual progress toward correct syntax but failed to address the fundamental flaws in binary search implementation and conditional logic.  There was no improvement in the core algorithm.

