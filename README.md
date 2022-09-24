## 49. Group Anagrams

Problem on LeetCode
https://leetcode.com/problems/group-anagrams/

## My youtube channel Where I make a full explanation and interpretation of the answers
https://www.youtube.com/watch?v=co8SuVnJ1uk&list=PL9bTI0hoGCu0d9FDJVpy_cpmwuOiLCVgb&index=5&pp=sAQB

### Method 

```python
    
class Solution:
    def groupAnagrams(self, strs: List[str]) -> List[List[str]]:
        h = {}
        for word in strs:
            sortedWord = ''.join(sorted(word))
            if sortedWord not in h:
                h[sortedWord] = [word]
            else:
                h[sortedWord].append(word)
        final = []
        for value in h.values():
            final.append(value)
        return final
```


          

