# Sparse Arrays

### Solution :smile:

```python
def matchingStrings(strings, queries):
    strMap = {}
    
    for s in strings:
        if s in strMap:
            strMap[s] += 1
        
        else:
            strMap[s] = 1
    
    result = []
    
    for i in range(len(queries)):
        if queries[i] in strMap:
            result.append(strMap[queries[i]])
            
        else:
            result.append(0)

    return result
```
