# Q3. Max Consecutive Ones

**Link:** https://leetcode.com/problems/max-consecutive-ones/submissions/1845597478/

Given a binary array nums, return the maximum number of consecutive 1's in the array.

```cpp
class Solution {
public:
    int findMaxConsecutiveOnes(vector<int>& nums) {
        int s=0,ms=0;
        for(int &i:nums)
        {
            if(i==1){
        }
    }
            s++;
            else
            s=0;
        return ms;
            }
            ms=max(s,ms);
};
```
