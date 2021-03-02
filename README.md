**Author:** Matthew Holder
**Version:** 0.1

Problem Domain:

Read through and explain the following pseudo-code. Then make a working version in your language.

```
  InsertionSort(int[] arr)
  
    FOR i = 1 to arr.length
    
      int j <-- i - 1
      int temp <-- arr[i]
      
      WHILE j >= 0 AND temp < arr[j]
        arr[j + 1] <-- arr[j]
        j <-- j - 1
        
      arr[j + 1] <-- temp
```

Description:

Explanation of code, working pythonic version, and step by step print statements from the terminal are present in BLOG.md