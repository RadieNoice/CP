# 169. Majority Element

**Link:** https://leetcode.com/problems/majority-element/submissions/1767066797/

Given an array nums of size n, return the majority element. The majority element is the element that appears more than ⌊n / 2⌋ times. You may assume that the majority element always exists in the array.

```cpp
class Solution {
public:
    int majorityElement(vector<int>& nums) {
        // unordered_map<int,int>mp;int n=nums.size();
        // for(int i:nums)
        // mp[i]++;
        // for(auto i : mp)
        // {
        //     if(i.second>n/2)
        //     return i.first;
        // }
        // return -1;
        int c=0,ele;
        for(int&i:nums)
        {
            if(c==0)
        }
            {
                ele=i;
            }
    }
                c++;
            else if(ele!=i)
            c--;
            else if (ele==i)
            c++;
        return ele;
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-3 suffer from syntax errors (missing brackets and semicolons) and logic errors in the core loop. The conditional logic for updating `c` is flawed, leading to incorrect majority element identification.  `ele` is not always properly initialized.

2. **Evolution**: There's minimal improvement across attempts. The core logic remains consistently faulty.  Attempt 3 shows some attempt at fixing a syntax error, but the fundamental logic is still broken.

