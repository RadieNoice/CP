# 229. Majority Element II

**Link:** https://leetcode.com/problems/majority-element-ii/submissions/1705809558/

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

TAGS: Logic Error, Conditional Logic, Loop Logic

1. **Key Issues**: Attempts 1-6 had unclosed brackets and incorrect conditional logic within the loop. Attempts 7-11  incorrectly handled candidate elements and their counts. Attempts 12-18 fixed logic but had off-by-one errors in final count checks and return conditions.

2. **Evolution**: The code evolved from a flawed single-candidate approach (attempts 1-6) to a more sophisticated two-candidate approach (attempts 7 onwards).  Attempts 12-18 correctly identified two candidates but struggled with accurate counting and return logic for edge cases, eventually fixing them in attempt 17-18.

