# Pangrams

### Solution :smile:
```java
    public static String pangrams(String s) {
        int[] mark = new int[26];
        String lowerCase = s.toLowerCase();
        for (int index = 0, i = 0; i < lowerCase.length(); i++) {
            if (Character.isLetter(lowerCase.charAt(i))) {
                index = lowerCase.charAt(i) - 'a';
                mark[index] = 1;
            }       
        }
        
        for (int i = 0; i < 26; i++) {
            if (mark[i] == 0) 
                return "not pangram";
        }
        
        return "pangram";
    }
```
