# 1. Two Sum

**Link:** https://leetcode.com/problems/two-sum/submissions/1693357219/

Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target. You may assume that each input would have exactly one solution, and you may not use the same element twice. You can return the answer in any order.

```cpp
        return x;
    //     unordered_map<int,int>mp;int n=nums.size();
    //     vector<int>arr;
    //     for(int i=0;i<n;i++)
            if(nums[i]==copy[k]||nums[j]==copy[k])
        }
    //     {
    //         int x=nums[i];
    //         int y=target-x;
    //         if(mp.find(y)!=mp.end())
        {
        for(int k=0;k<n;k++)
        }
            break;
            if (x==target)
            j--;
            if(x>target)
            i++;
            if(x<target)
            int x=nums[i]+nums[j];
        {
        vector<int>x;
            x.emplace_back(k);
            if(x.size()==2)
            break;
```

## Mistake Analysis

TAGS: Logic Error, Algorithm Choice, Loop Logic

1. **Key Issues**: Attempts 1-13 incorrectly implemented a two-pointer approach after sorting, failing to handle cases properly and using `find` inefficiently. Attempts 14-15 tried a brute-force approach with flawed logic for duplicate detection.  None correctly used a hash map.

2. **Evolution**: Initial attempts showed flawed two-pointer logic. Later attempts moved towards a hash map approach but struggled with index retrieval and duplicate handling.  No attempt successfully implemented a correct and efficient solution.

