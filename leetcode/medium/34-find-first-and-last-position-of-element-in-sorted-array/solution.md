# 34. Find First and Last Position of Element in Sorted Array

**Link:** https://leetcode.com/problems/find-first-and-last-position-of-element-in-sorted-array/

Given an array of integers nums sorted in non-decreasing order, find the starting and ending position of a given target value. If target is not found in the array, return [-1, -1]. You must write an algorithm with O(log n) runtime complexity.

```cpp
·‌·‌·‌·‌·‌·‌·‌·‌int·‌l=0,r=nums.size()-1,m,s=-1,e=-1;
·‌·‌·‌·‌·‌·‌·‌·‌while(l<=r)
·‌·‌·‌·‌·‌·‌·‌·‌{
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌m=(l+r)/2;
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌if(nums[m]==target)
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌{
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌int·‌i=m;
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌while(i>=0&&nums[i]==target)
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌i--;
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌s=i+1;
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌i=m;
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌while(i<=nums.size()-1&&nums[i]==target)
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌i++;
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌e=i-1;
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌break;
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌}
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌if(nums[m]<=target)
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌l=m+1;
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌else
·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌·‌r=m-1;·‌·‌·‌·‌·‌·‌·‌·‌
·‌·‌·‌·‌·‌·‌·‌·‌}
·‌·‌·‌·‌·‌·‌·‌·‌return·‌vector<int>{s,e};
·‌·‌·‌·‌}
};
·‌·‌·‌·‌vector<int>·‌searchRange(vector<int>&·‌nums,·‌int·‌target)·‌{
public:
class·‌Solution·‌{
```
