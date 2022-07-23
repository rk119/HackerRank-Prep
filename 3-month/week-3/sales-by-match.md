# Sales by Match

### Solution :smile:
```java
    public static int sockMerchant(int n, List<Integer> ar) {
        HashMap<Integer, Integer> hs = new HashMap<Integer, Integer>();
        for (int i = 0; i < n; i++) {
            int num = ar.get(i);
            if (hs.containsKey(num)) hs.put(num, hs.get(num)+1);
            else hs.put(num, 1);
        }
        
        int count = 0;
        for (int i = 0; i < n; i++) {
            int num = ar.get(i);   
            if (hs.get(num) >= 2) { 
                hs.put(num, hs.get(num)-2); 
                count++; 
            }                   
        }        
        
        return count;        
    }
```
