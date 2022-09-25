## 344. Reverse String
Problem on LeetCode
https://leetcode.com/problems/reverse-string/

## My youtube channel Where I make a full explanation and interpretation of the answers
https://youtu.be/KGUiTqNChkg

### Method 1 
```python
class Solution:
    def reverseString(self, s: List[str]) -> None:
        """
        Do not return anything, modify s in-place instead.
        """
        l,r=0,len(s)-1
        while l<r:
            s[l],s[r]=s[r],s[l]
            l,r=l+1,r-1
```

### Method 2 

```python
class Solution:
    def reverseString(self, s: List[str]) -> None:
        """
        Do not return anything, modify s in-place instead.
        """
        s[:] = s[::-1]
```

### Method 3 : stack

```python
    
class Solution:
    def reverseString(self, s: List[str]) -> None:
        """
        Do not return anything, modify s in-place instead.
        """
        stack = []
        for c in s :
            stack.append(c)
        i=0
        while stack:
            s[i]=stack.pop()
            i +=1
        
        
        
```




          

