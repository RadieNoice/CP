# 3304. Find the K-th Character in String Game I

**Link:** https://leetcode.com/problems/find-the-k-th-character-in-string-game-i/

Alice and Bob are playing a game. Initially, Alice has a string word = "a". You are given a positive integer k. Now Bob will ask Alice to perform the following operation forever: Generate a new string by changing each character in word to its next character in the English alphabet, and append it to the original word.

```cpp
class Solution {
public:
    char kthCharacter(int k) {
       string s="a";int t=log2(k);
        {
            t+=(i-'a'+1)%26+'a';
        }
    }
       return s[k-1];
        cout<<s<<endl;
        for(auto i:s)
       while(s.size()<=pow(2,t+1)){
       }
        string t="";
        s+=t;
       cout<<t;
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Array Bounds

1. **Key Issues**: Attempts 1-4 had off-by-one errors and used `s[-1]` incorrectly. Attempts 5-21 used incorrect logic for string generation and failed to implement the iterative string expansion.  Incorrect array indexing (`s[k-1]`, `s[k]`) led to out-of-bounds access.

2. **Evolution**: Early attempts focused on the basic string manipulation; later attempts incorrectly tried to use logarithms to predict string length, leading to more complex errors.  No attempt correctly implemented the core string-building logic.

