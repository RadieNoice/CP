# 485. Max Consecutive Ones

**Link:** https://leetcode.com/problems/max-consecutive-ones/submissions/1755629636/

Given a binary array nums, return the maximum number of consecutive 1's in the array.

```cpp
        //     if(i==1)
        //     {
        //         cs++;
        //         ms=max(cs,ms);
        //     }
        //     else
        //     cs=0;
        // {
        // for(int i: nums)
        // int ms=0,cs=0;
        return ms;
        // }
        // return ms;
        // nums.emplace_back(0);
        // int n=nums.size(),c=0,x=0;
        }
            s=0;
            else
            }
            s++;
            ms=max(s,ms);
            if(nums[i]==1){
        {
        for(int i=0;i<n;i++)
        int n=nums.size();int ms=0,s=0;
    int findMaxConsecutiveOnes(vector<int>& nums) {
public:
        // for(int i=0;i<n-1;i++)
        // {
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-6 suffer from incorrect conditional logic and incomplete loop logic.  The `if/else if` structure doesn't correctly handle consecutive ones; index `i+1` causes array out of bounds.  Attempt 7 has a better loop, but misses resetting `s`.


2. **Evolution**: The code gradually shifts from a flawed conditional approach to a more structured loop in attempt 7.  However, even attempt 7 lacks complete logic to correctly reset the counter `s`.  Debugging output was added but didn't resolve the core logic flaws.

