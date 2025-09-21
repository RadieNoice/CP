# 153. Find Minimum in Rotated Sorted Array

**Link:** https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/submissions/1777766599/

```cpp
class Solution {
public:
    int findMin(vector<int>& nums) {
        int l=0,r=nums.size()-1,m,ans=INT_MAX;
        while(l<=r)
        {
            m=(l+r)/2;
        }
            if(nums[l]<=nums[m])

            {
                ans=min(ans,nums[l]);
            }
                l=m+1;
            else
            {
                ans=min(ans,nums[m]);
            }
    }
                r=m-1;
        return ans;
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempt 1 and 2 both have a `while` loop missing its body.  The conditional logic within the loop is flawed; it doesn't correctly identify the minimum element.  `max` is incorrectly used instead of `min` to update `ans`. The loop updates `l` and `r` incorrectly, outside the `if-else` block.

2. **Evolution**: Attempt 2 corrects the use of `min` instead of `max` function.  However, both attempts fail to implement the binary search correctly to find the minimum element in a rotated sorted array.

