# Plus Minus

### Solution :smile:
```python
def plusMinus(arr):
    length, positives, negatives, zeros = len(arr), 0, 0, 0 
    for i in arr:
        if i > 0:
            positives+=1
        elif i == 0:
            zeros+=1
        else:
            negatives+=1
    
    print("{0: .6f}".format((positives/length)))
    print("{0: .6f}".format((negatives/length)))
    print("{0: .6f}".format((zeros/length)))

```
