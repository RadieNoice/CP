# 3307. Find the K-th Character in String Game II

**Link:** https://leetcode.com/problems/find-the-k-th-character-in-string-game-ii/submissions/1697735529/

Alice and Bob are playing a game. Initially, Alice has a string word = "a". You are given a positive integer k. You are also given an integer array operations, where operations[i] represents the type of the ith operation. Now Bob will ask Alice to perform all operations in sequence: If operations[i] == 0, append a copy of word to itself.

```cpp
class Solution {
public:
    int shift(long long k,vector<int>&op)
    {
        if(k<=(long long)1) return 0;
        long long t=log2(k),a=k-(1LL<<t);
        if(a==0){
            return op[t-1]+shift(1LL<<(t-1LL),op);
        }
        else{
            return op[t]+shift(a,op);
        }
    }
    char kthCharacter(long long k, vector<int>& operations) {
        return 97+(shift(k,operations))%26;
        // string str="a";
        
        // for(int i=0;i<operations.size();i++)
        // {
        //     if (str.length() >= k) {
        //         break;
        //     }
        //     if(operations[i]==0)
        //     {
        //         str+=str;
        //     }
        //     if(operations[i]==1)
        //     {
```
