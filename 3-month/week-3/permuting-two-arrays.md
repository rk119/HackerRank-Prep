# Permuting Two Arrays

### Solution :smile:
```java
    public static String twoArrays(int k, List<Integer> A, List<Integer> B) {
        Collections.sort(A);
        Collections.sort(B);
        
        for (int a = 0, b = B.size() - 1; a < A.size() && b >= 0; a++, b--) {
            if (A.get(a) + B.get(b) < k) 
                return "NO";
        }
        
        return "YES";
    }
```
