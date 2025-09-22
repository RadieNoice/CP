# 3005. Count Elements With Maximum Frequency

**Link:** https://leetcode.com/problems/count-elements-with-maximum-frequency/submissions/1778541063/

You are given an array nums consisting of positive integers. Return the total frequencies of elements in nums such that those elements all have the maximum frequency. The frequency of an element is the number of occurrences of that element in the array.

```cpp
class Solution {
public:
    int maxFrequencyElements(vector<int>& nums) {
        unordered_map <int,int>mp;int m=INT_MIN,c=0;
        for(int&i:nums){
        mp[i]++;
        m=max(m,mp[i]);
        }
        for(auto&i:mp)
        {
            if(i.second==m)
        }
    }
            c+=i.second;
        return c;

};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic

1. **Key Issues**: All attempts fail to correctly increment `c` within the `if` block.  The `c+=i.second;` statement is improperly placed outside the loop's scope in attempts 1-6.  Attempt 2 incorrectly multiplies `c`.

2. **Evolution**: Attempts progressively correct the initialization of `c` and attempt to add `i.second`.  However, the crucial placement of `c+=i.second` within the conditional remains flawed until the final attempt (which still has the placement error).

