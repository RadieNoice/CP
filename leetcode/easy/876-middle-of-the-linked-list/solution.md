# 876. Middle of the Linked List

**Link:** https://leetcode.com/problems/middle-of-the-linked-list/submissions/1720456429/

Given the head of a singly linked list, return the middle node of the linked list. If there are two middle nodes, return the second middle node.

```cpp
 *     ListNode() : val(0), next(nullptr) {}
 *     ListNode(int x) : val(x), next(nullptr) {}
 *     ListNode(int x, ListNode *next) : val(x), next(next) {}
 * };
 */
class Solution {
public:
    ListNode* middleNode(ListNode* head) {
        int t=0;ListNode*temp=head;
        while(temp!=nullptr)
        {
            temp=temp->next;
        }
            t++;
        t/=2;t++;
        while(true)
        {
            t--;
            temp=temp->next;
        }
    }
        temp=head;
        return temp;
            if(t==0)
            break;
};
```
