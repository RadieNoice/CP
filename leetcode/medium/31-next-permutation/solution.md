# 31. Next Permutation

**Link:** https://leetcode.com/problems/next-permutation/submissions/1695315242/

A permutation of an array of integers is an arrangement of its members into a sequence or linear order.

```cpp
class Solution {
public:
    void nextPermutation(vector<int>& nums) {
        next_permutation(nums.begin(),nums.end());
    }
};
```

## Mistake Analysis

TAGS: Algorithm Choice

1. **Key Issues**: Attempt 1 directly uses `next_permutation`,  avoiding the core problem of implementing the algorithm. It lacks the logic to find and generate the next lexicographical permutation.

2. **Evolution**: No evolution shown as only one attempt is provided.  The solution is trivial and doesn't demonstrate any iterative problem-solving.

