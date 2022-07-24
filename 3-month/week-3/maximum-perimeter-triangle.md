# Maximum Perimeter Triangle

### Solution :smile:
```java
    public static List<Integer> maximumPerimeterTriangle(List<Integer> sticks) {
        Collections.sort(sticks);
        int i = sticks.size() - 3;
        
        while (i >= 0 && (sticks.get(i) + sticks.get(i+1) <= sticks.get(i+2))) 
            i--;
            
        if (i >= 0) 
            return List.of(sticks.get(i), sticks.get(i+1), sticks.get(i+2));
        
        return List.of(-1); 
    }
```
