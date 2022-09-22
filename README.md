242. Valid Anagram
Problem on LeetCode
https://leetcode.com/problems/valid-anagram/

## My youtube channel Where I make a full explanation and interpretation of the answers
https://www.youtube.com/watch?v=hI6dDj0OEg8&list=PL9bTI0hoGCu0d9FDJVpy_cpmwuOiLCVgb&index=3&pp=sAQB

### Method 1 --  hashtable

```python
    
class Solution:
    def isAnagram(self, s: str, t: str) -> bool:
        if len(s) != len(t):
            return False
        
        dic1 , dic2 = {} , {}
        
        for item in s:
            dic1[item] = dic1.get(item,0) +1
        for item in t:
            dic2[item] = dic2.get(item,0) +1
        return dic1 == dic2
```     

 ### Method 2 -- Sorting
 
```python
    
class Solution:
    def isAnagram(self, s: str, t: str) -> bool:
        return sorted(s) == sorted(t)
        
```


          

