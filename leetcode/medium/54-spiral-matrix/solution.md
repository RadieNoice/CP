# 54. Spiral Matrix

**Link:** https://leetcode.com/problems/spiral-matrix/submissions/1697384785/

Given an m x n matrix, return all elements of the matrix in spiral order.

```cpp
class Solution {
public:
    vector<int> spiralOrder(vector<vector<int>>& matrix) {
        vector<int>ans;int n=matrix.size(),m=matrix[0].size(),t=0,b=n-1,l=0,r=m-1;
        while(t<=b&&l<=r)
        {
            for(int i=l;i<=r;i++)
        }
            ans.emplace_back(matrix[t][i]);
            for(int i=t;i<=b;i++)
            t++;
            ans.emplace_back(matrix[i][r]);
            r--;
                for(int i=r;i>=l;i--)
                ans.emplace_back(matrix[b][i]);
                b--;
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌for(int·‌i=b;i>=t;i--)
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌ans.emplace_back(matrix[i][l]);
    }
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌l++;
        return ans;
            if(t<=b){
            }
            if(l<=r){
            }
};
```
