# 77. Combinations

**Link:** https://leetcode.com/problems/combinations/submissions/1831360524/

Given two integers n and k, return all possible combinations of k numbers chosen from the range [1, n]. You may return the answer in any order.

```cpp
class Solution {
public:
    void recurse(vector<int>x,vector<vector<int>>&y,int index,int k,int j){
        if(index==k)

    }
    vector<vector<int>> combine(int n, int k) {
        vector<int>x;
        {
            for(int i=0;i<k;i++)
        
            vector<int> temp;
            temp.push_back(x[i]);
            return;
            for(int i=j;i<x.size();i++)
            {
                swap(x[index],x[i]);
            }
    }
                recurse(x,y,index+1,k,i+1);
                swap(x[index],x[i]);
        vector<vector<int>>y;
        for(int i=1;i<=n;i++)
        x.push_back(i);
        recurse(x,y,0,k,0);
        return y;
    }
            y.push_back(temp);
};
```
