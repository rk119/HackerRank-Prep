# Divisible Sum Pairs

### Solution :smile:

```python
def divisibleSumPairs(n, k, ar):
    counter=0
    for i in range(n):
        for j in range(i+1,n):
            addn=ar[i]+ar[j]
            if addn%k ==0:
                counter=counter+1
                    
```
