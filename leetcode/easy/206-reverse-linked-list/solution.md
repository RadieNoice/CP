# 206. Reverse Linked List

**Link:** https://leetcode.com/problems/reverse-linked-list/

Given the head of a singly linked list, reverse the list, and return the reversed list.

```cpp
/**
 * Definition for singly-linked list.
 * struct ListNode {
 *     int val;
 *     ListNode *next;
 *     ListNode() : val(0), next(nullptr) {}
 *     ListNode(int x) : val(x), next(nullptr) {}
 *     ListNode(int x, ListNode *next) : val(x), next(next) {}
 * };
 */
class Solution {
public:
    ListNode* reverseList(ListNode* head) {
        ListNode*x=head,*y=head,*z=nullptr;
        {
            z=y->next;
            y->next=x;
            x=y;
        }
        return x;
    }
            y=z;
        while(y->next!=nullptr); 
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Null Pointer

1. **Key Issues**: Attempts 1-6 had syntax errors and undefined variables. Attempts 7-17 lacked proper loop logic and didn't handle the `nullptr` head case correctly. Attempt 18 is incomplete.  The core issue was incorrect iterative reversal logic.

2. **Evolution**: The code progressed from nonsensical syntax to a partially correct iterative approach, repeatedly failing due to missing initialization, incorrect loop conditions, and improper pointer manipulation.  Attempt 13 was closest but still incomplete.

