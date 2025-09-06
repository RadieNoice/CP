# 75. Sort Colors

**Link:** https://leetcode.com/problems/sort-colors/submissions/1761230017/

Given an array nums with n objects colored red, white, or blue, sort them in-place so that objects of the same color are adjacent, with the colors in the order red, white, and blue. We will use the integers 0, 1, and 2 to represent the color red, white, and blue, respectively. You must solve this problem without using the library's sort function.

```cpp
    //         i++;
    //         j++;
    //         }
    //         swap(nums[i],nums[j]);
    //         if(nums[j]==0){
    //     {
    //     while(j<=k)
    //     int i=0,n=nums.size(),k=n-1,j=0;
            j++;
        }
    //     //Dutch National Law Algorithm
            else
            }
            else if(nums[j]==2)
            {
                swap(nums[j],nums[k]);
                k--;
            }
                i++;j++;
                swap(nums[j],nums[i]);
            if(nums[j]==0)
            {
    //         else if(nums[j]==2)
    //         {
    //             swap(nums[k],nums[j]);
    //             k--;
    //         }
    //         else
    //             j++;
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-4 suffer from incomplete or incorrect implementation of the Dutch National Flag algorithm.  Conditional logic within the `while` loop is flawed, leading to incorrect swapping and incomplete sorting.  Increment/decrement of `i`, `j`, `k` are improperly handled.

2. **Evolution**:  The attempts show a progression towards the correct algorithm, but the logic within the loop consistently fails to correctly handle all three color cases simultaneously.  The code remains incomplete and buggy throughout all attempts.

