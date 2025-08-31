# 75. Sort Colors

**Link:** https://leetcode.com/problems/sort-colors/submissions/1754518469/

Given an array nums with n objects colored red, white, or blue, sort them in-place so that objects of the same color are adjacent, with the colors in the order red, white, and blue. We will use the integers 0, 1, and 2 to represent the color red, white, and blue, respectively. You must solve this problem without using the library's sort function.

```cpp
    //         i++;
    //         swap(nums[i],nums[j]);
    //         if(nums[j]==0){
    //     {
    //     while(j<=k)
    //     int i=0,n=nums.size(),k=n-1,j=0;
    //     //Dutch National Law Algorithm
    }
    //         j++;
        }
            j++;
            else
            }
                swap(nums[j],nums[k]);
                k--;
            {
            }
            else if(nums[j]==2)
                swap(nums[i],nums[j]);
                i++;j++;
            if(nums[j]==0)
            {
        {
        while(j<=k)
    void sortColors(vector<int>& nums) {
        int i=0,j=0,k=nums.size()-1;
class Solution {
public:
```

## Mistake Analysis

TAGS: Logic Error, Syntax Error, Loop Logic

1. **Key Issues**: Attempt 1 & 3 have syntax errors (e.g., `nums.szie()`, misplaced braces). Attempt 1, 2, and 3 have logic errors in their `while` loop;  incorrect increment/decrement of `i`, `j`, `k`, leading to incorrect swaps and incomplete sorting.

2. **Evolution**: Attempt 2 corrects the `nums.size()` syntax error.  However, the fundamental logic error in the three-way partitioning remains. None of the attempts correctly implement the Dutch National Flag algorithm.

