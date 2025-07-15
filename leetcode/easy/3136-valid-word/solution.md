# 3136. Valid Word

**Link:** https://leetcode.com/problems/valid-word/submissions/1698501133/

A word is considered valid if: It contains a minimum of 3 characters. It contains only digits (0-9), and English letters (uppercase and lowercase). It includes at least one vowel. It includes at least one consonant. You are given a string word. Return true if word is valid, otherwise, return false. Notes: 'a', 'e', 'i', 'o', 'u', and their uppercases are vowels. A consonant is an English letter that is not a vowel.

```cpp
class Solution {
public:
    bool isValid(string word) {
        if(word.size()<3)
        return false;
        regex a("[aeiou]+");
        regex c("[\\W]");
        return regex_search(word,b)&&!regex_search(word,c)&&regex_search(word,a);
    }
        transform(word.begin(), word.end(), word.begin(), ::tolower);
        regex b("[bcdfghjklmnpqrstvwxyz]+");
};
```

## Mistake Analysis

TAGS: Logic Error, Syntax Error, Algorithm Choice

1. **Key Issues**: Attempts 1-3 were incomplete. Attempts 4-24 struggled with regex syntax for correctly identifying all conditions (length, vowels, consonants, alphanumeric characters). Attempt 25 had a syntax error in lookahead assertion. Attempts 26-30 lacked complete vowel/consonant checks.

2. **Evolution**:  The solution progressed from incomplete code to using regex for validation.  The regex was refined across several attempts, improving towards the correct combination of character classes and quantifiers. The final attempts incorporated explicit length and character checks.

