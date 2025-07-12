# 31. Next Permutation

**Link:** https://leetcode.com/problems/next-permutation/submissions/1695505961/

A permutation of an array of integers is an arrangement of its members into a sequence or linear order.

```cpp
class Solution {
public:
    void nextPermutation(vector<int>& nums) {

        int n= nums.size(),t=-1;
        for(int i=n-2;i>=0;i--)
        {
            if(nums[i+1]>nums[i])
            {
        }
        // next_permutation(nums.begin(),nums.end());
            }
                t=i;break;
        if(t==-1)
        sort(nums.begin(),nums.end());
        else
        {
            for(int i=n-1;i>t;i--)
        }
            {
                if(nums[i]>nums[t]){
            }
    }
                swap(nums[i],nums[t]);
                break;}
            sort(nums.begin()+t+1,nums.end());
};
```
