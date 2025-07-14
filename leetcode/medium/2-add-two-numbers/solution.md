# 2. Add Two Numbers

**Link:** https://leetcode.com/problems/add-two-numbers/submissions/1697290428/

You are given two non-empty linked lists representing two non-negative integers. The digits are stored in reverse order, and each of their nodes contains a single digit. Add the two numbers and return the sum as a linked list. You may assume the two numbers do not contain any leading zero, except the number 0 itself.

```cpp
public:
    ListNode* addTwoNumbers(ListNode* l1, ListNode* l2) {
 *     ListNode(int x, ListNode *next) : val(x), next(next) {}
 * };
 */
class Solution {
        ListNode* s=new ListNode(),*l3=s;int c=0;
        while(l1||l2)
        {
            if(l1)
        }
            int sum=c;
            {
                sum+=l1->val;
            }
                l1=l1->next;
            if(l2)
            {
                sum+=l2->val;
            }
                l2=l2->next;
        return l3->next;
            s->next=new ListNode(sum%10);s=s->next;
    }
            cout<<sum<<" "<<sum%10<<" "<<c<<endl;
            c=sum/10;
        if(c!=0)
        s->next=new ListNode(c);
};
```

## Mistake Analysis

TAGS: Logic Error, Null Pointer, Loop Logic

1. **Key Issues**: Attempts 1-4 had incomplete loops and returned an integer instead of a ListNode. Attempts 5-55 failed to correctly handle carry and null pointer dereferences;  loop conditions were flawed. Attempt 56 correctly added numbers but didn't handle carry in the last node.

2. **Evolution**:  The code gradually progressed towards a correct structure, with later attempts using a proper linked list and addressing carry.  The final attempt (56) nearly solved the problem, needing only a slight adjustment to the carry handling and return value.

