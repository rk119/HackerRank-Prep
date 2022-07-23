# Counting Sort 1

### Solution :smile:
```java
    public static List<Integer> countingSort(List<Integer> arr) {
        int[] freq = new int[100];
        Arrays.fill(freq, 0);
        for (int value : arr) {
            freq[value]++;
        }
        
        List<Integer> list = new ArrayList<>();
        for (int e : freq) {
            list.add(e);
        }
        return list;
    }
```
