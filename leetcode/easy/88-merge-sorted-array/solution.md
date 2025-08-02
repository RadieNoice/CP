# 88. Merge Sorted Array

**Link:** https://leetcode.com/problems/merge-sorted-array/submissions/1720380665/

You are given two integer arrays nums1 and nums2, sorted in non-decreasing order, and two integers m and n, representing the number of elements in nums1 and nums2 respectively. Merge nums1 and nums2 into a single array sorted in non-decreasing order. The final sorted array should not be returned by the function, but instead be stored inside the array nums1. To accommodate this, nums1 has a length of m + n, where the first m elements denote the elements that should be merged, and the last n elements are set to 0 and should be ignored. nums2 has a length of n.

```cpp
class Solution {
public:
    void merge(vector<int>& nums1, int m, vector<int>& nums2, int n) {
        int j=0,i=m;
        while(j<n)
        {
           auto x= lower_bound(nums1.begin(),nums1.begin()+i,nums2[j]);
           if(x!=nums1.end()){
           nums1.insert(x,nums2[j]);
           else
           {
            nums1[i++]=nums2[j];
           j++;
        }
    }
           }
           nums1.pop_back();
           for(int k:nums1)
           cout<<k<<" ";
           cout<<endl;
           cout<<"  "<<j<<"  "<<i;
           }
           i++;
};
```

## Mistake Analysis

TAGS: Logic Error, Algorithm Choice, Loop Logic

1. **Key Issues**: Attempts 1-17 incorrectly used `nums1.insert()`,  increasing vector size and causing index issues.  Attempts 18-53 used `lower_bound` but had logic errors in handling insertion and the loop termination condition.  The correct approach is to merge from the end of `nums1` efficiently.

2. **Evolution**: Initial attempts tried inefficient insertions. Later attempts used `lower_bound` for a better approach, although they still had flawed loop control and insertion logic.  The attempts progressively tried fixing the insertion issues.

