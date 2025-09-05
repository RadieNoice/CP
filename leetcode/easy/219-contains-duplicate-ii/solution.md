# 219. Contains Duplicate II

**Link:** https://leetcode.com/problems/contains-duplicate-ii/submissions/1760784280/

Given an integer array nums and an integer k, return true if there are two distinct indices i and j in the array such that nums[i] == nums[j] and abs(i - j) <= k.

```cpp
class Solution {
public:
    bool containsNearbyDuplicate(vector<int>& nums, int k) {
        int n=nums.size();
        for(int i=0;i<n;i++)
        {
            for(int j=i+1;j<=i+k &&j<n;j++)
        }
            {
                if(nums[i]==nums[j])
            }
    }
        return false;
                return true;
};
```

## Mistake Analysis

TAGS: Loop Logic, Conditional Logic, Array Bounds

1. **Key Issues**: Attempts 1-17 had unclosed `if` statements and incorrect loop bounds, failing to check all pairs within `k` distance.  Attempt 19 compared `i` to itself. Attempt 21 and 22 lacked a mechanism to return `true` outside nested loops.

2. **Evolution**: Attempts gradually corrected loop conditions and bounds (`<=`, `<`).  Attempts introduced `min` to track minimum distance but failed to initialize return value correctly within the loop; they also improperly tried to return true.  The final attempts still had logic errors in returning `true`.

