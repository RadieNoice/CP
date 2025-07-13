# 3304. Find the K-th Character in String Game I

**Link:** https://leetcode.com/problems/find-the-k-th-character-in-string-game-i/

Alice and Bob are playing a game. Initially, Alice has a string word = "a". You are given a positive integer k. Now Bob will ask Alice to perform the following operation forever: Generate a new string by changing each character in word to its next character in the English alphabet, and append it to the original word.


## Mistake Analysis

TAGS: Logic Error, Off By One, Algorithm Choice

1. **Key Issues**: All attempts except the last one incorrectly calculate the k-th character. The logic to generate the string and find the k-th character is missing and replaced by flawed approximations using `log2(k)`.  Off-by-one errors in character calculation are present in multiple attempts.

2. **Evolution**: Attempts progressively refine the incorrect formula, trying different offsets and modulo operations to map the logarithm result to the alphabet. The final attempt is incomplete but closer to the correct approach.

