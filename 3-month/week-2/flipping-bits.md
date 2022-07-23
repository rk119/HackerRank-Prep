# Flipping Bits

### Solution :smile:
```java
    public static long flippingBits(long n) {
        return ~n & 0x00000000ffffffffL;
    }
```
