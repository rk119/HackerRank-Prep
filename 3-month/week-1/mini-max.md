# Mini Max

### Solution :smile:

```python

def miniMaxSum(arr):
    length = len(arr)
    if length < 5:
        raise Exception("Array needs to have 5 or more elements")
    
    arr.sort()
    i, j, minimum, maximum = 0, length-1, 0, 0
    while (i < 4):
        minimum += arr[i]
        maximum += arr[j]
        i += 1
        j -= 1
        
    print("{} {}".format(minimum, maximum))
```
