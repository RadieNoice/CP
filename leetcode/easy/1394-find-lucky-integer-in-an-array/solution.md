# 1394. Find Lucky Integer in an Array

**Link:** https://leetcode.com/problems/find-lucky-integer-in-an-array/description/

Given an array of integers arr, a lucky integer is an integer that has a frequency in the array equal to its value. Return the largest lucky integer in the array. If there is no lucky integer return -1.

```cpp
class Solution {
public:
    int findLucky(vector<int>& arr) {
        unordered_map<int,int>maps;int t=0;
        map<int,int>mapss;
        for(int i : arr)
        maps[i]++;
        for(auto i:maps)
        {
            if(i.first==i.second)
            mapss[i.first]++;
        }
        if(mapss.empty())return -1;
        auto i=mapss.rbegin();
        return i->first;
    }
};
```
