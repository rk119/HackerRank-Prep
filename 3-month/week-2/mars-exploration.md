# Mars Exploration

### Solution :smile:
```java
    public static int marsExploration(String s) {
        int numMessages = s.length() / 3;
        String compare = "SOS".repeat(numMessages);
        int faults = 0;
        
        for (int i = 0; i < s.length(); i++) {
            if (compare.charAt(i) != s.charAt(i))
                faults++;
        }
        
        return faults;
    }
```
