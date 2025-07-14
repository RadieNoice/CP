# 75. Sort Colors

**Link:** https://leetcode.com/problems/sort-colors/description/

Given an array nums with n objects colored red, white, or blue, sort them in-place so that objects of the same color are adjacent, with the colors in the order red, white, and blue. We will use the integers 0, 1, and 2 to represent the color red, white, and blue, respectively. You must solve this problem without using the library's sort function.

```cpp
            i++;
            j++;
            }
            else if(nums[j]==2)
            {
                swap(nums[k],nums[j]);
                k--;
            }
            else
                j++;
        }
        
        // map<int,int>mp;
        // for(int i:nums)
        // mp[i]++;
        // nums.clear();
        // for(auto i:mp)
        // {
        //     for(int j=0;j<i.second;j++)
            swap(nums[i],nums[j]);
            if(nums[j]==0){
        //     nums.emplace_back(i.first);
        // }
        
    }
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempt 1 has incomplete and incorrect nested loops for the three-way partitioning.  The `if-else if-else` conditions are logically flawed, leading to incorrect swapping and an infinite loop in some cases.  The commented-out map approach is a correct alternative but was not implemented.

2. **Evolution**: No further attempts were provided for analysis of improvement.

