# Q2. Shuffle the Array

**Link:** https://leetcode.com/problems/shuffle-the-array/submissions/1845593922/

Given the array nums consisting of 2n elements in the form [x1,x2,...,xn,y1,y2,...,yn]. Return the array in the form [x1,y1,x2,y2,...,xn,yn].

```cpp
class Solution {
public:
    vector<int> shuffle(vector<int>& nums, int n) {
        vector<int>ans(2*n);
        for(int i=0,j=0;i<2*n;i+=2,j++)
            ans[i]=nums[j];
        for(int i=1,j=n;i<2*n;i+=2,j++)
        return ans;
    }
            ans[i]=nums[j];
};
```
