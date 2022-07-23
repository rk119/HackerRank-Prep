# Counting Valleys

### Solution :smile:
```java
    public static int countingValleys(int steps, String path) {
        int numValleys = 0;
        for (int alt = 0, i = 0; i < steps; i++) {
            char c = path.charAt(i);
            if (c == 'U') {
                alt++;
                if (alt == 0)
                    numValleys++;
            }
            else
                alt--;         
        }
        return numValleys;
    }
```
