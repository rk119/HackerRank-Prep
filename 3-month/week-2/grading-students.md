### Solution :smile:
```java
 public static List<Integer> gradingStudents(List<Integer> grades) {
        List<Integer> list = new ArrayList<>();
        for (int i = 0; i < grades.size(); i++) {
            int value = grades.get(i);
            int remainder = value % 5;
            if (value >= 38 && (((value+5) - remainder) - value) < 3) {
                list.add(((value+5) - remainder));
            }
            else {
                list.add(value);
            }
        }
        return list;
    }
```
