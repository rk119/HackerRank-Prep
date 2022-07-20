# Lonely Integer

### Solutions :smile:

```java
    public static int lonelyinteger(List<Integer> a) {
        // 1 - 0001
        //     0000
        // XOR=0001
        // 2 - 0010
        // XOR=0011
        // 3 - 0011
        // XOR=0000
        // 4 - 0100
        // XOR=0100
        // 3 - 0011
        // XOR=0111
        // 2 - 0010
        // XOR=0101
        // 1 - 0001
        // XOR=0100  = 4 
        int result = 0;
        for (int i = 0; i < a.size(); i++) {
            result ^= a.get(i);
        }     
        return result;
    }
```
