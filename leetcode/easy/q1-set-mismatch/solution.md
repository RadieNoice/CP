# Q1. Set Mismatch

**Link:** https://leetcode.com/problems/set-mismatch/submissions/1845610070/

You have a set of integers s, which originally contains all the numbers from 1 to n. Unfortunately, due to some error, one of the numbers in s got duplicated to another number in the set, which results in repetition of one number and loss of another number. You are given an integer array nums representing the data status of this set after the error. Find the number that occurs twice and the number that is missing and return them in the form of an array.

```cpp
class Solution {
public:
    vector<int> findErrorNums(vector<int>& nums) {
        int n=nums.size(),m=n*(n+1)/2,l=0;
        for(int &i:nums)
        l+=i;
        ranges::sort(nums);
        for(int i=0;i<n-1;i++)
        {
            if(nums[i]==nums[i+1])
            {
                l-=nums[i];
                return vector<int>{nums[i],m-l};
            }
        }
        return vector<int>{};

    }
};
```
