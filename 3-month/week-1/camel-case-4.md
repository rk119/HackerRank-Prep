# Camel Case 4

### Solution :smile:

```python
import re
while True:
    try:
        inp = input().strip()
        op, typ, text = inp.split(";")
        if op == "S":
            if typ == "M":
                text = text[:-2]                                       
            arr = re.findall('.[^A-Z]*', text)
            
            result = ""
            for i in arr:
                result += (i.lower() + " ")
            
            print(result)
                
        if op == "C":
            text = text.split(" ")
            result = ""
            
            if typ == "V":
                result = text[0]
                for i in range(1, len(text)):
                    result += text[i][0].upper() + text[i][1:]
            
            elif typ == "C":
                for i in text:
                    result += i[0].upper() + i[1:]
                    
            else:  
                result = text[0]
                for i in range(1, len(text)):
                    result += text[i][0].upper() + text[i][1:]    
                result += '()'
                
            
            print(result)
```
