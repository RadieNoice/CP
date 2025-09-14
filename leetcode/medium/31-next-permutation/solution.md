# 31. Next Permutation

**Link:** https://leetcode.com/problems/next-permutation/description/

A permutation of an array of integers is an arrangement of its members into a sequence or linear order.

```cpp
        // int n= nums.size(),t=-1;
        // for(int i=n-2;i>=0;i--)
        // {
        //     if(nums[i+1]>nums[i])
        //     {
        }
        }
        sort(nums.begin()+t+1,nums.end());
            break;}
            swap(nums[i],nums[t]);
        //         t=i;break;
        //     }
        // }
        // if(t==-1)
        // sort(nums.begin(),nums.end());
        // else
        // {
        //     for(int i=n-1;i>t;i--)
        //     {
        //         if(nums[i]>nums[t]){
        //         swap(nums[i],nums[t]);
        //         break;}
        //     }
        //     sort(nums.begin()+t+1,nums.end());
        // }
        // next_permutation(nums.begin(),nums.end());
    }
};
```

## Mistake Analysis

TAGS: Logic Error, Loop Logic, Conditional Logic

1. **Key Issues**: Attempts 1-3 contain numerous syntax errors and unclosed brackets, rendering them uncompilable.  The core logic for finding the pivot and swapping elements is incomplete and contains logical flaws in conditional statements and loop boundaries. Attempt 4 is commented out, showing the coder likely understood the algorithm but struggled with implementation.

2. **Evolution**: The code evolved from a completely broken state towards a potentially functional solution (though still commented out in Attempt 4).  The attempts show progressive refinement but never achieve a syntactically correct and logically sound implementation.

