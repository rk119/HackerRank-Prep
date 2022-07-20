# Time Conversion

### Solution :smile:

```python
def timeConversion(s):
    if (s[-2] == 'P' and not s[0:2] == '12'):
        s = str(12 + int(s[0:2])) + s[2:-2]
    elif (s[-2] == 'A' and s[0:2] == '12'):
        s = '00' + s[2:-2]
    else:
        s = s[:-2]
    
    return s
```
