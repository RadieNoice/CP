# 3304. Find the K-th Character in String Game I

**Link:** https://leetcode.com/problems/find-the-k-th-character-in-string-game-i/submissions/1697735077/

Alice and Bob are playing a game. Initially, Alice has a string word = "a". You are given a positive integer k. Now Bob will ask Alice to perform the following operation forever: Generate a new string by changing each character in word to its next character in the English alphabet, and append it to the original word.

```cpp
class Solution {
public:
    int shift(int k)
    {
        if(k<=1)return 0;
        int t=log2(k),a=k-(1<<t);
        if(a==0)
        return 1+ shift((1<<t)-1);
        else
        return 1+ shift(a);

    }
    char kthCharacter(int k){
        return 97+shift(k);
    //    string s="a";int t=log2(k);
    //    while(s.size()<=pow(2,t+1)){
    //     string t="";
    //     for(auto i:s)
    //     {
    //         t+=(i-'a'+1)%26+'a';
    //     }
    //     s+=t;
    //     cout<<s<<endl;
    //    }
    //    cout<<t;
    //    return s[k-1];
    }
};
```
