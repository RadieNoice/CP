# 1290. Convert Binary Number in a Linked List to Integer

**Link:** https://leetcode.com/problems/convert-binary-number-in-a-linked-list-to-integer/submissions/1697236792/

Given head which is a reference node to a singly-linked list. The value of each node in the linked list is either 0 or 1. The linked list holds the binary representation of a number. Return the decimal value of the number in the linked list. The most significant bit is at the head of the linked list.

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
    int getDecimalValue(ListNode* head) {
        int s=0,j=0;vector<int>v;
        while(head!=nullptr)
        {
        }
    }
            head=head->next;
        return s;
            v.emplace_back(head->val);
        for(auto i=v.rbegin();i!=v.rend();++i)
        s+=pow(2,j++)*(*i);
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Null Pointer

1. **Key Issues**: Attempts 1-4 had incorrect `sample` usage;  `sample` was not updated correctly within the loop. Attempts 5-8 failed to correctly iterate through the linked list and calculate the decimal value. Attempts 9-17 had logic errors in vector handling and iteration (incorrect loop conditions, `emplace_back` on `head->next` instead of `head->val`). Attempt 18 corrected the increment operator in the for loop.

2. **Evolution**:  The code gradually moved towards correct linked list traversal.  Attempt 18 finally corrected the vector manipulation and loop logic, but  still potentially suffers from integer overflow if the binary number is too large.

