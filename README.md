## 217. Contains Duplicate 
Problem on LeetCode
https://leetcode.com/problems/contains-duplicate/

## My youtube channel Where I make a full explanation and interpretation of the answers
https://www.youtube.com/watch?v=hI6dDj0OEg8&list=PL9bTI0hoGCu0d9FDJVpy_cpmwuOiLCVgb&index=3&pp=sAQB

### Method 1 --  hashtable

```python
    
class Solution:
    
    def containsDuplicate(self, nums: List[int]) -> bool:        
        hashNum = {}
        for i in nums :
            if i not in hashNum:
                hashNum[i] = i
            else:
                return True                                             
        return False 
```     

 ### Method 2 -- Sorting
 
```python
    
class Solution:
    
    def containsDuplicate(self, nums: List[int]) -> bool:
        nums.sort()
        for i in range(1,len(nums)):
            if nums[i] == nums[i-1]:
                return True
        return False
```


          

