# 206. Reverse Linked List

**Link:** https://leetcode.com/problems/reverse-linked-list/submissions/1720450980/

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
        ListNode*x=nullptr,*y=head,*z=nullptr;
        {
            z=y->next;
            x=y;
        }
        return x;
    }
            y=z;
        while(y!=nullptr) 
            y->next=x;
};
```

## Mistake Analysis

TAGS: Logic Error, Null Pointer, Loop Logic

1. **Key Issues**: Attempts 1-6 all failed to correctly implement the iterative reversal algorithm.  Attempts 1-3 had a null pointer dereference (`y->next`) initially. Attempts 4-6 didn't properly update pointers within the loop, missing the core logic of reversing the links.  The `while` loop was also misplaced and incomplete.

2. **Evolution**: Attempts progressed toward correct pointer initialization (`x=nullptr, y=head`).  Attempt 6 correctly returned `x` (the new head), but the loop remained flawed. The core algorithm was never fully implemented in any attempt.

