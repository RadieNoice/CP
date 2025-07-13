# 2410. Maximum Matching of Players With Trainers

**Link:** https://leetcode.com/problems/maximum-matching-of-players-with-trainers/submissions/1696145070/

You are given a 0-indexed integer array players, where players[i] represents the ability of the ith player. You are also given a 0-indexed integer array trainers, where trainers[j] represents the training capacity of the jth trainer. The ith player can match with the jth trainer if the player's ability is less than or equal to the trainer's training capacity. Additionally, the ith player can be matched with at most one trainer, and the jth trainer can be matched with at most one player. Return the maximum number of matchings between players and trainers that satisfy these conditions.

```cpp
class Solution {
public:
    int matchPlayersAndTrainers(vector<int>& players, vector<int>& trainers) {
        sort(players.begin(),players.end());
        sort(trainers.begin(),trainers.end());
        for(int i:players)
        cout<<i<<" ";
        cout<<endl;
        for(int i:trainers)
        cout<<i<<" ";
        cout<<endl;
        int c=0,p=0,t=0,ps=players.size(),ts=trainers.size();
        while(p<ps&&t<ts)
        {
            if(players[p]<=trainers[t]){
            c++;
            p++;t++;
            }
            else
            t++;
        }
        return c;
    }
};
```

## Mistake Analysis

TAGS: Algorithm Choice, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-3 incorrectly sorted `trainers` in descending order, leading to wrong matches. Attempt 4 fixed sorting but had a logic error in the `else` condition; it should increment `p` if the player's ability is too high, not `t`.

2. **Evolution**: Attempts progressed towards correct sorting.  Attempt 4 identified and corrected the sorting issue but introduced a different logic error in the `while` loop's conditional branch.  The final attempt shows a better understanding of sorting but has a remaining loop logic issue.

