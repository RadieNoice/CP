# 3304. Find the K-th Character in String Game I

**Link:** https://leetcode.com/problems/find-the-k-th-character-in-string-game-i/submissions/1696205975/

Alice and Bob are playing a game. Initially, Alice has a string word = "a". You are given a positive integer k. Now Bob will ask Alice to perform the following operation forever: Generate a new string by changing each character in word to its next character in the English alphabet, and append it to the original word.

```cpp
        else
        return 1+ shift(a);

    }
    char kthCharacter(int k){
    //    string s="a";int t=log2(k);
    //    while(s.size()<=pow(2,t+1)){
    //     string t="";
    //     for(auto i:s)
    //     {
    //         t+=(i-'a'+1)%26+'a';
    //     }
    //     s+=t;
        return 97+shift(k);
        return 1+ shift((1<<t)-1);
        if(a==0)
        int t=log2(k),a=k-(1<<t);
        if(k<=1)return 0;
    {
    int shift(int k)
public:
class Solution {
    //     cout<<s<<endl;
    //    }
    //    cout<<t;
    //    return s[k-1];
    }
};
```

## Mistake Analysis

TAGS: Logic Error, Conditional Logic, Algorithm Choice

1. **Key Issues**: The `shift` function is recursively defined but never correctly utilized within `kthCharacter`.  Attempts incorrectly calculate the character shift based on flawed logic for handling the recursive steps and string generation.  The algorithm fundamentally misunderstands the problem's pattern.

2. **Evolution**: Attempts iteratively tried to fix the recursive calls and conditional logic within `shift` and `kthCharacter`, but without a correct understanding of the pattern of string growth, they failed to produce a working solution.  The commented-out code hints at a more appropriate approach (iterative string building), which was never fully implemented.

