# Q2. Shuffle the Array

**Link:** https://leetcode.com/problems/shuffle-the-array/submissions/1845595624/

Given the array nums consisting of 2n elements in the form [x1,x2,...,xn,y1,y2,...,yn]. Return the array in the form [x1,y1,x2,y2,...,xn,yn].

```cpp
class Solution {
public:
    vector<int> shuffle(vector<int>& nums, int n) {
        vector<int>ans;
        for(int i=0;i<n;i++){
        ans.emplace_back(nums[i]);
        ans.emplace_back(nums[i+n]);
        return ans;
    }
        }
};
```
