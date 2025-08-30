# 36. Valid Sudoku

**Link:** https://leetcode.com/problems/valid-sudoku/submissions/1753502373/

Determine if a 9 x 9 Sudoku board is valid. Only the filled cells need to be validated according to the following rules: Each row must contain the digits 1-9 without repetition. Each column must contain the digits 1-9 without repetition. Each of the nine 3 x 3 sub-boxes of the grid must contain the digits 1-9 without repetition.

```cpp
            for(int j=0;j<9;j++)
            unordered_map<char,int>mp;
        {
        for(int i=0;i<9;i++)
    {
    }
    bool check_col(vector<vector<char>>& b)
        return true;
        }
            return false;
            if(!check(mp))
            }
                mp[b[i][j]]++;
            {
            unordered_map<char,int>mp;
            for(int j=0;j<9;j++)
        {
        for(int i=0;i<9;i++)
    {
    bool check_row(vector<vector<char>>& b)
    }

        return false;
        return true;
        if(check_row(b)&&check_col(b)&&check_box(b))
    bool isValidSudoku(vector<vector<char>>& b) {
public:
class Solution {
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempt 1 is incomplete (missing `check_box` and `check` function implementations).  The `check_col` function iterates incorrectly; it should iterate through columns, not rows.  Conditional logic within `check_row` doesn't handle '.' (empty cells) correctly.

2. **Evolution**: No evolution is shown as the code is incomplete.  The provided snippet shows a flawed approach to column checking, and lacks crucial parts to determine validity.

