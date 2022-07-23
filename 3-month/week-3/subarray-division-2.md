# Subarray Division 2

### Solution :smile:
```java
    public static int birthday(List<Integer> s, int d, int m) {
        int count = 0;
        int sum = 0;
        
        if(m <= s.size()) { 
            for(int i = 0; i < m; i++) {
                sum += s.get(i);
            }
        }
        
        if(sum == d) 
            count++;
            
        for(int i = 0; i < s.size()-m; i++) {
            sum = sum - s.get(i) + s.get(i+m);
            if(sum == d) 
                count++;
        }
        
        return count;
    }
```
