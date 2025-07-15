# 3136. Valid Word

**Link:** https://leetcode.com/problems/valid-word/submissions/1698502586/

A word is considered valid if: It contains a minimum of 3 characters. It contains only digits (0-9), and English letters (uppercase and lowercase). It includes at least one vowel. It includes at least one consonant. You are given a string word. Return true if word is valid, otherwise, return false. Notes: 'a', 'e', 'i', 'o', 'u', and their uppercases are vowels. A consonant is an English letter that is not a vowel.

```cpp
class Solution {
public:
    bool isValid(string word) {
        if(word.size()<3)
        return false;
        regex a("[aeiou]+",regex_constants::icase);
        regex c("[\\W]");
        return regex_search(word,b)&&!regex_search(word,c)&&regex_search(word,a);
    }
        regex b("[bcdfghjklmnpqrstvwxyz]+",regex_constants::icase);
};
```

## Mistake Analysis

TAGS: Logic Error, Syntax Error, Conditional Logic

1. **Key Issues**: Attempt 1 has several issues: `regex b` is undeclared in the scope where it's used. The regex `c`  (`[\\W]`) matches any non-alphanumeric character, not just consonants. The logic `!regex_search(word,c)` incorrectly checks for the *absence* of non-alphanumeric characters instead of requiring only alphanumeric ones.  The vowel and consonant checks are insufficiently combined.


2. **Evolution**: No further attempts were provided for analysis.

