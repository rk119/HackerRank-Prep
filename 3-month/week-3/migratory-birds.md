# Migratory Birds

### Solution :smile:
```java
    public static int migratoryBirds(List<Integer> arr) {
        Collections.sort(arr);
        HashMap<Integer, Integer> hs = new HashMap<Integer, Integer>();
        int counter = 0;
        int max = 0;
        for (int i = 0; i < arr.size(); i++) {
            int num = arr.get(i);
            if (hs.containsKey(num)) hs.put(num, hs.get(num)+1);
            else hs.put(num, 1);
            
            if (hs.get(num) > counter) {
                max = num;
                counter = hs.get(num);
            }
        }
        
        return max;
    }
```
