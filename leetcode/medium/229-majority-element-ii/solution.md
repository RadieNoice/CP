# 229. Majority Element II

**Link:** https://leetcode.com/problems/majority-element-ii/submissions/1705809671/

Given an integer array of size n, find all elements that appear more than ⌊ n/3 ⌋ times.

```cpp
            x++;
            if(i==ele2)
            y++;
            if(i==ele1)
        {
        for(int i:nums)
        }
            }
                cnt1--;cnt2--;
            else{
            else if(i==ele2)cnt2++;
            else if(i==ele1)cnt1++;
            }
                cnt2++;
        }
        if(x>n/3&&y>n/3)
        return vector<int>{ele1,ele2};
        else if(x>n/3)
        return vector<int>{ele1};
        else if(y>n/3) return vector<int>{ele2};
        // int n=nums.size();vector<int>ans;
        // n/=3;
        // cout<<n;
        // unordered_map<int,int>mp;
        // for(int i:nums){
        // mp[i]++;
        // }
        // for(auto i:mp)
        else return vector<int>{};
```

## Mistake Analysis

TAGS: Logic Error, Conditional Logic

1. **Key Issues**: Attempts 1-6 had incorrect conditional logic and missing code. Attempts 7-11 failed to update `ans` and had logic errors in handling the two potential majority elements. Attempts 12-18 fixed most logic errors but had issues with the `>=` vs `>` comparison and handling empty return vectors.

2. **Evolution**:  The code evolved from a flawed single-element approach to a two-element approach using Boyer-Moore's voting algorithm, but with errors in conditional statements and final result handling.  The final attempts largely corrected the logic, improving the accuracy of the algorithm.

