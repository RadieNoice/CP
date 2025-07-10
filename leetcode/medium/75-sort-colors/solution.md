# 75. Sort Colors

**Link:** https://leetcode.com/problems/sort-colors/submissions/1693367161/

Given an array nums with n objects colored red, white, or blue, sort them in-place so that objects of the same color are adjacent, with the colors in the order red, white, and blue. We will use the integers 0, 1, and 2 to represent the color red, white, and blue, respectively. You must solve this problem without using the library's sort function.

```cpp
class Solution {
public:
    void sortColors(vector<int>& nums) {
        map<int,int>mp;
        for(int i:nums)
        mp[i]++;
        nums.clear();
        for(auto i:mp)
        {
            for(int j=0;j<i.second;j++)
        }
    }
            nums.emplace_back(i.first);
        
};
```

## Mistake Analysis

TAGS: Logic Error, Data Structure, Loop Logic

1. **Key Issues**: All attempts incorrectly clear the input vector `nums`.  The nested loops to reconstruct `nums` are incomplete and have misplaced `nums.emplace_back()` and `return nums` statements. Using a `map` is inefficient for this problem.

2. **Evolution**: Attempts 1 and 2 show progression in syntax (using auto in the range-based for loop), but the core logic flaw remains. Attempt 3 removes the invalid `return` statement.  None correctly implement in-place sorting.

