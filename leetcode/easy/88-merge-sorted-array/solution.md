# 88. Merge Sorted Array

**Link:** https://leetcode.com/problems/merge-sorted-array/submissions/1720387406/

You are given two integer arrays nums1 and nums2, sorted in non-decreasing order, and two integers m and n, representing the number of elements in nums1 and nums2 respectively. Merge nums1 and nums2 into a single array sorted in non-decreasing order. The final sorted array should not be returned by the function, but instead be stored inside the array nums1. To accommodate this, nums1 has a length of m + n, where the first m elements denote the elements that should be merged, and the last n elements are set to 0 and should be ignored. nums2 has a length of n.

```cpp
class Solution {
public:
    void merge(vector<int>& nums1, int m, vector<int>& nums2, int n) {
        // int j=0,i=m;
        // while(j<n)
        // {
        //    auto x= lower_bound(nums1.begin(),nums1.begin()+i,nums2[j]);
        //    if(x!=nums1.end()){
        //    nums1.insert(x,nums2[j]);
        //    nums1.pop_back();
        //    i++;
        int i=0,j=0;
        while(i<m+n&&j<n)
        {
        }
            if(nums1[i]>=nums2[j])
            {
                nums1.insert(nums1.begin()+i,nums2[j]);
            }
                nums1.pop_back();
                i++;
                j++;
            else if (nums1[i]==0){
            nums1[i]=nums2[j];
            }
            i++;j++;
            else i++;
        sort(nums1.begin(),nums1.end());
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-11 had a flawed `while` loop and incorrect conditional logic for merging elements; `nums1.pop_back()` was misused. Attempt 12 sorted the array after, inefficiently.  The core logic of merging sorted arrays was not implemented.

2. **Evolution**:  Attempts progressed towards correct `nums1.insert()` usage and a more structured `if-else if` statement.  The final attempt used `sort`, showing a lack of understanding of merging sorted arrays.  However, the loop and conditional logic remained fundamentally flawed.

