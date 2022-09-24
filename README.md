## 796. Rotate String
Problem on LeetCode
https://leetcode.com/problems/rotate-string/

## My youtube channel Where I make a full explanation and interpretation of the answers
https://www.youtube.com/watch?v=wF0TyEsmNO4&list=PL9bTI0hoGCu0d9FDJVpy_cpmwuOiLCVgb&index=4&pp=sAQB

### Method 

```python
    
class Solution:
    def rotateString(self, s: str, goal: str) -> bool:
               
        return len(s) == len(goal) and goal in s+s
        
```


          

