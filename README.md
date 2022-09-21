## 1. Two Sum
Problem on LeetCode
https://leetcode.com/problems/two-sum/

My youtube channel Where I make a full explanation and interpretation of the answers <br/>
https://www.youtube.com/watch?v=r8z506Ox3zM&list=PL9bTI0hoGCu0d9FDJVpy_cpmwuOiLCVgb&index=1&t=460s

### Method 1 --  Brute Force

```python
    
class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        
        for i in range(len(nums)):
            for j in range(i+1 , len(nums)):
                if nums[j] == target - nums[i]:
                    return [i,j]
        
                                                         
                
```     
### Method 2 --  Hash Table


```python

class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        
        hashtab = {}
        for i in range(len(nums)):
            cond = target - nums[i]
            if cond in hashtab:
                return [i ,hashtab[cond]]
            hashtab[nums[i]] = i
        
        
        
          
```
