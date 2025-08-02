# 206. Reverse Linked List

**Link:** https://leetcode.com/problems/reverse-linked-list/submissions/1720451108/

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
