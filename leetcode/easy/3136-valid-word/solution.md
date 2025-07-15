# 3136. Valid Word

**Link:** https://leetcode.com/problems/valid-word/submissions/1698509712/

A word is considered valid if: It contains a minimum of 3 characters. It contains only digits (0-9), and English letters (uppercase and lowercase). It includes at least one vowel. It includes at least one consonant. You are given a string word. Return true if word is valid, otherwise, return false. Notes: 'a', 'e', 'i', 'o', 'u', and their uppercases are vowels. A consonant is an English letter that is not a vowel.

```cpp
class Solution {
public:
    bool isValid(string word) {
        for(auto i :word)
        {
            if(!isalnum(i))
            return false;
            if(isalpha(i))
            {
                i=tolower(i);
            }
        }
        // if(word.size()<3)
        // return false;
        // regex a("[aeiou]+",regex_constants::icase);
        // regex b("[bcdfghjklmnpqrstvwxyz]+",regex_constants::icase);
        // regex c("[\\W]");
        // return regex_search(word,b)&&!regex_search(word,c)&&regex_search(word,a);
    }
                if(i=='a'||i=='e'||i=='i'||i=='o'||i=='u')
        bool v=false,c=false;
                v=true;
                else
                c=true;
        if(word.size()<3)
        return false;
        return c&v;
};
```

## Mistake Analysis

TAGS: Logic Error, Conditional Logic

1. **Key Issues**: Attempts 1-6 had incorrect vowel/consonant logic; `v` and `c` were not properly initialized and updated within the loop. Attempt 7 partially fixed initialization but the logic for setting `v` and `c` was still flawed.  The length check (`word.size()<3`) was inconsistently placed and never actually used.

2. **Evolution**: Attempts gradually improved input validation (`isalnum`, `isalpha`). The initialization of `v` and `c` was addressed in Attempt 7, but the core vowel/consonant check remains fundamentally flawed and unimplemented.  The code never actually checked the whole string for vowels and consonants.

