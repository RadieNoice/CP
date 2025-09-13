# 3541. Find Most Frequent Vowel and Consonant

**Link:** https://leetcode.com/problems/find-most-frequent-vowel-and-consonant/

You are given a string s consisting of lowercase English letters ('a' to 'z'). Your task is to: Find the vowel (one of 'a', 'e', 'i', 'o', or 'u') with the maximum frequency. Find the consonant (all other letters excluding vowels) with the maximum frequency. Return the sum of the two frequencies.


## Mistake Analysis

TAGS: Logic Error, Data Structure, Variable Initialization

1. **Key Issues**: Attempt 1 has syntax errors (`vint mv=0,mc=0;` and uses `v` before declaration). Attempt 2 fixes syntax but incorrectly initializes `mv` and `mc` outside the loop; `v` is used to track both vowels and consonants, leading to incorrect max frequency calculation.

2. **Evolution**: Attempt 2 corrected the syntax errors of Attempt 1. However, it still suffers from a logic error in calculating the maximum frequencies.  Both attempts failed to correctly track and utilize map data structures to find maximum frequencies.

