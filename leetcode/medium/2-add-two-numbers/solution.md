# 2. Add Two Numbers

**Link:** https://leetcode.com/problems/add-two-numbers/

You are given two non-empty linked lists representing two non-negative integers. The digits are stored in reverse order, and each of their nodes contains a single digit. Add the two numbers and return the sum as a linked list. You may assume the two numbers do not contain any leading zero, except the number 0 itself.

```cpp
    ListNode* addTwoNumbers(ListNode* l1, ListNode* l2) {
        ListNode* s=new ListNode(),*l3=s;int c=0;
        while(l1||l2)
        {
            int sum=c;
            if(l1)
            {
                sum+=l1->val;
                l1=l1->next;
            }
            if(l2)
            {
                sum+=l2->val;
                l2=l2->next;
            }
            s->next=new ListNode(sum%10);s=s->next;
            c=sum/10;
            //cout<<sum<<" "<<sum%10<<" "<<c<<endl;
        }
        if(c!=0)
        s->next=new ListNode(c);
        return l3->next;
public:
class Solution {
 */
 * };
 *     ListNode(int x, ListNode *next) : val(x), next(next) {}
 *     ListNode(int x) : val(x), next(nullptr) {}
```
