# 2149. Rearrange Array Elements by Sign

**Link:** https://leetcode.com/problems/rearrange-array-elements-by-sign/

You are given a 0-indexed integer array nums of even length consisting of an equal number of positive and negative integers. You should return the array of nums such that the the array follows the given conditions: Every consecutive pair of integers have opposite signs. For all integers with the same sign, the order in which they were present in nums is preserved. The rearranged array begins with a positive integer. Return the modified array after rearranging the elements to satisfy the aforementioned conditions.

```cpp
class Solution {
public:
    vector<int> rearrangeArray(vector<int>& nums) {
        vector<int>p,n,a;int s=nums.size();
        for(int i:nums)
        {
            if(i<0)
        }
            n.emplace_back(i);
            else
            p.emplace_back(i);
        for(int i=0;i<s/2;i++)
        {
            a.emplace_back(p[i]);
        }
·‌·‌·‌·‌}
            a.emplace_back(n[i]);
        return·‌a;
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempt 1 and 2 are missing closing braces for the `if` and `for` statements.  The loop logic within the `for` loop incorrectly appends positive and negative numbers alternately; it only appends half of each. Conditional logic within the `if` statement is also incomplete, not handling positive numbers correctly.

2. **Evolution**: No actual evolution; both attempts have identical core logic flaws.  Neither attempt compiles or runs correctly.

