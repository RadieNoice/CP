# 875. Koko Eating Bananas

**Link:** https://leetcode.com/problems/koko-eating-bananas/submissions/1777201220/

Koko loves to eat bananas. There are n piles of bananas, the ith pile has piles[i] bananas. The guards have gone and will come back in h hours. Koko can decide her bananas-per-hour eating speed of k. Each hour, she chooses some pile of bananas and eats k bananas from that pile. If the pile has less than k bananas, she eats all of them instead and will not eat any more bananas during this hour. Koko likes to eat slowly but still wants to finish eating all the bananas before the guards return. Return the minimum integer k such that she can eat all the bananas within h hours.

```cpp
            }
                if(i<=k)
                t++;
                else
                {
                }
                    if(i%k==0)
                    t+=i/k;
                    else
                    t+=i/k+1;
            if(t<=h){
            //cout<<t<<endl;
                ans=k;
            r=k-1;
            }
            else if(t>h)
            l=k+1;
            
        }
        return ans;
    }
};
```

## Mistake Analysis

TAGS: Logic Error, Algorithm Choice, Conditional Logic

1. **Key Issues**: Attempts 1 & 2 only calculated the average speed, ignoring hourly constraints. Attempts 3-19 had incorrect binary search conditions (`t>k` instead of `t>h`) and missing or incorrect return statements.  Attempt 20 fixed the conditional logic, but not the variable initialization.

2. **Evolution**: The code gradually implemented a binary search to find the minimum speed.  Incorrect conditional logic in the binary search was progressively corrected, culminating in a functional solution in Attempt 20.  Type of `t` was also improved.

