# Diagonal Difference

### Solution :smile:
```java
    public static int diagonalDifference(List<List<Integer>> arr) {
        int len = arr.size();
        int ltor = 0, rtol = 0, j = 0, k = len-1;
        for (int i = 0; i < len; i++) {
            ltor += (arr.get(i)).get(j);
            rtol += (arr.get(i)).get(k);
            j++;
            k--;
        }
        

        int max = ltor > rtol ? ltor : rtol;
        int min = ltor < rtol ? ltor : rtol;
        return (max-min);
    }
```
