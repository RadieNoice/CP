# 3477. Fruits Into Baskets II

**Link:** https://leetcode.com/problems/fruits-into-baskets-ii/submissions/1724724156/

You are given two arrays of integers, fruits and baskets, each of length n, where fruits[i] represents the quantity of the ith type of fruit, and baskets[j] represents the capacity of the jth basket. From left to right, place the fruits according to these rules: Each fruit type must be placed in the leftmost available basket with a capacity greater than or equal to the quantity of that fruit type. Each basket can hold only one type of fruit. If a fruit type cannot be placed in any basket, it remains unplaced. Return the number of fruit types that remain unplaced after all possible allocations are made.

```cpp
class Solution {
public:
    int numOfUnplacedFruits(vector<int>& fruits, vector<int>& baskets) {
        int n=fruits.size(),j=0,k=0;
        for(int i=0;i<n;i++)
        {
            if(fruits[i]<=baskets[j]){
        }
            baskets[j]=-1;j++;
            else
            {
            }
                for(int k=j;k<n;k++)
                {
                    if(fruits[i]<=baskets[k]){
    }
                }
                int t=true;
                    t=false;baskets[k]=-1;break;}
                if(t)
                k++;
            }
        return k;
};
```
