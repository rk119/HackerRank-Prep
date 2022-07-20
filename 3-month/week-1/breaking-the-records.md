# Breaking The Records

### Solution :smile:

```python
def breakingRecords(scores):
    result = [0, 0]
    maximum = scores[0]
    minimum = scores[0]
    for i in range(1, len(scores)):
        if scores[i] > maximum:
            result[0] += 1
            maximum = scores[i]
        
        if scores[i] < minimum:
            result[1] += 1
            minimum = scores[i]            
    
    return result
```
