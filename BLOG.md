In the first loop we use the second loop to evaluate whether or not there is a number after the current index which is smaller than the number at the current index. If there is the two values switch places.

```
def insertion(l):
  for i in range(len(l)):
    for j in range(len(l)):
      if l[j] > l[i]:
        l[j],l[i] = l[i],l[j]
  return l
```

Results:
```
[20, 18, 12, 8, 5, -2]
[20, 18, 12, 8, 5, -2]
[20, 18, 12, 8, 5, -2]
[20, 18, 12, 8, 5, -2]
[20, 18, 12, 8, 5, -2]
[20, 18, 12, 8, 5, -2]
[20, 18, 12, 8, 5, -2]
[18, 20, 12, 8, 5, -2]
[18, 20, 12, 8, 5, -2]
[18, 20, 12, 8, 5, -2]
[18, 20, 12, 8, 5, -2]
[18, 20, 12, 8, 5, -2]
[18, 20, 12, 8, 5, -2]
[12, 20, 18, 8, 5, -2]
[12, 18, 20, 8, 5, -2]
[12, 18, 20, 8, 5, -2]
[12, 18, 20, 8, 5, -2]
[12, 18, 20, 8, 5, -2]
[12, 18, 20, 8, 5, -2]
[8, 18, 20, 12, 5, -2]
[8, 12, 20, 18, 5, -2]
[8, 12, 18, 20, 5, -2]
[8, 12, 18, 20, 5, -2]
[8, 12, 18, 20, 5, -2]
[8, 12, 18, 20, 5, -2]
[5, 12, 18, 20, 8, -2]
[5, 8, 18, 20, 12, -2]
[5, 8, 12, 20, 18, -2]
[5, 8, 12, 18, 20, -2]
[5, 8, 12, 18, 20, -2]
[5, 8, 12, 18, 20, -2]
[-2, 8, 12, 18, 20, 5]
[-2, 5, 12, 18, 20, 8]
[-2, 5, 8, 18, 20, 12]
[-2, 5, 8, 12, 20, 18]
[-2, 5, 8, 12, 18, 20]
[-2, 5, 8, 12, 18, 20]

[5, 12, 7, 5, 5, 7]
[5, 12, 7, 5, 5, 7]
[12, 5, 7, 5, 5, 7]
[12, 5, 7, 5, 5, 7]
[12, 5, 7, 5, 5, 7]
[12, 5, 7, 5, 5, 7]
[12, 5, 7, 5, 5, 7]
[5, 12, 7, 5, 5, 7]
[5, 12, 7, 5, 5, 7]
[5, 12, 7, 5, 5, 7]
[5, 12, 7, 5, 5, 7]
[5, 12, 7, 5, 5, 7]
[5, 12, 7, 5, 5, 7]
[5, 12, 7, 5, 5, 7]
[5, 7, 12, 5, 5, 7]
[5, 7, 12, 5, 5, 7]
[5, 7, 12, 5, 5, 7]
[5, 7, 12, 5, 5, 7]
[5, 7, 12, 5, 5, 7]
[5, 7, 12, 5, 5, 7]
[5, 5, 12, 7, 5, 7]
[5, 5, 7, 12, 5, 7]
[5, 5, 7, 12, 5, 7]
[5, 5, 7, 12, 5, 7]
[5, 5, 7, 12, 5, 7]
[5, 5, 7, 12, 5, 7]
[5, 5, 7, 12, 5, 7]
[5, 5, 5, 12, 7, 7]
[5, 5, 5, 7, 12, 7]
[5, 5, 5, 7, 12, 7]
[5, 5, 5, 7, 12, 7]
[5, 5, 5, 7, 12, 7]
[5, 5, 5, 7, 12, 7]
[5, 5, 5, 7, 12, 7]
[5, 5, 5, 7, 12, 7]
[5, 5, 5, 7, 7, 12]
[5, 5, 5, 7, 7, 12]

[3, 2, 5, 7, 13, 11]
[3, 2, 5, 7, 13, 11]
[3, 2, 5, 7, 13, 11]
[5, 2, 3, 7, 13, 11]
[7, 2, 3, 5, 13, 11]
[13, 2, 3, 5, 7, 11]
[13, 2, 3, 5, 7, 11]
[2, 13, 3, 5, 7, 11]
[2, 13, 3, 5, 7, 11]
[2, 13, 3, 5, 7, 11]
[2, 13, 3, 5, 7, 11]
[2, 13, 3, 5, 7, 11]
[2, 13, 3, 5, 7, 11]
[2, 13, 3, 5, 7, 11]
[2, 3, 13, 5, 7, 11]
[2, 3, 13, 5, 7, 11]
[2, 3, 13, 5, 7, 11]
[2, 3, 13, 5, 7, 11]
[2, 3, 13, 5, 7, 11]
[2, 3, 13, 5, 7, 11]
[2, 3, 13, 5, 7, 11]
[2, 3, 5, 13, 7, 11]
[2, 3, 5, 13, 7, 11]
[2, 3, 5, 13, 7, 11]
[2, 3, 5, 13, 7, 11]
[2, 3, 5, 13, 7, 11]
[2, 3, 5, 13, 7, 11]
[2, 3, 5, 13, 7, 11]
[2, 3, 5, 7, 13, 11]
[2, 3, 5, 7, 13, 11]
[2, 3, 5, 7, 13, 11]
[2, 3, 5, 7, 13, 11]
[2, 3, 5, 7, 13, 11]
[2, 3, 5, 7, 13, 11]
[2, 3, 5, 7, 13, 11]
[2, 3, 5, 7, 11, 13]
[2, 3, 5, 7, 11, 13]
```

To change it to a reverse sort we can change the comparing sign in the if statement to check if `l[i] > l[j]`.

```
def insertion(l):
  for i in range(len(l)):
    for j in range(len(l)):
      if l[j] < l[i]:
        l[j],l[i] = l[i],l[j]
  return l
```

Results:
```
[20, 18, 12, 8, 5, -2]
[20, 18, 12, 8, 5, -2]
[18, 20, 12, 8, 5, -2]
[12, 20, 18, 8, 5, -2]
[8, 20, 18, 12, 5, -2]
[5, 20, 18, 12, 8, -2]
[-2, 20, 18, 12, 8, 5]
[20, -2, 18, 12, 8, 5]
[20, -2, 18, 12, 8, 5]
[20, -2, 18, 12, 8, 5]
[20, -2, 18, 12, 8, 5]
[20, -2, 18, 12, 8, 5]
[20, -2, 18, 12, 8, 5]
[20, -2, 18, 12, 8, 5]
[20, 18, -2, 12, 8, 5]
[20, 18, -2, 12, 8, 5]
[20, 18, -2, 12, 8, 5]
[20, 18, -2, 12, 8, 5]
[20, 18, -2, 12, 8, 5]
[20, 18, -2, 12, 8, 5]
[20, 18, -2, 12, 8, 5]
[20, 18, 12, -2, 8, 5]
[20, 18, 12, -2, 8, 5]
[20, 18, 12, -2, 8, 5]
[20, 18, 12, -2, 8, 5]
[20, 18, 12, -2, 8, 5]
[20, 18, 12, -2, 8, 5]
[20, 18, 12, -2, 8, 5]
[20, 18, 12, 8, -2, 5]
[20, 18, 12, 8, -2, 5]
[20, 18, 12, 8, -2, 5]
[20, 18, 12, 8, -2, 5]
[20, 18, 12, 8, -2, 5]
[20, 18, 12, 8, -2, 5]
[20, 18, 12, 8, -2, 5]
[20, 18, 12, 8, 5, -2]
[20, 18, 12, 8, 5, -2]

[12, 5, 7, 5, 5, 7]
[12, 5, 7, 5, 5, 7]
[5, 12, 7, 5, 5, 7]
[5, 12, 7, 5, 5, 7]
[5, 12, 7, 5, 5, 7]
[5, 12, 7, 5, 5, 7]
[5, 12, 7, 5, 5, 7]
[12, 5, 7, 5, 5, 7]
[12, 5, 7, 5, 5, 7]
[12, 5, 7, 5, 5, 7]
[12, 5, 7, 5, 5, 7]
[12, 5, 7, 5, 5, 7]
[12, 5, 7, 5, 5, 7]
[12, 5, 7, 5, 5, 7]
[12, 7, 5, 5, 5, 7]
[12, 7, 5, 5, 5, 7]
[12, 7, 5, 5, 5, 7]
[12, 7, 5, 5, 5, 7]
[12, 7, 5, 5, 5, 7]
[12, 7, 5, 5, 5, 7]
[12, 7, 5, 5, 5, 7]
[12, 7, 5, 5, 5, 7]
[12, 7, 5, 5, 5, 7]
[12, 7, 5, 5, 5, 7]
[12, 7, 5, 5, 5, 7]
[12, 7, 5, 5, 5, 7]
[12, 7, 5, 5, 5, 7]
[12, 7, 5, 5, 5, 7]
[12, 7, 5, 5, 5, 7]
[12, 7, 5, 5, 5, 7]
[12, 7, 5, 5, 5, 7]
[12, 7, 5, 5, 5, 7]
[12, 7, 5, 5, 5, 7]
[12, 7, 7, 5, 5, 5]
[12, 7, 7, 5, 5, 5]
[12, 7, 7, 5, 5, 5]
[12, 7, 7, 5, 5, 5]

[3, 2, 5, 7, 13, 11]
[3, 2, 5, 7, 13, 11]
[2, 3, 5, 7, 13, 11]
[2, 3, 5, 7, 13, 11]
[2, 3, 5, 7, 13, 11]
[2, 3, 5, 7, 13, 11]
[2, 3, 5, 7, 13, 11]
[3, 2, 5, 7, 13, 11]
[3, 2, 5, 7, 13, 11]
[3, 2, 5, 7, 13, 11]
[3, 2, 5, 7, 13, 11]
[3, 2, 5, 7, 13, 11]
[3, 2, 5, 7, 13, 11]
[5, 2, 3, 7, 13, 11]
[5, 3, 2, 7, 13, 11]
[5, 3, 2, 7, 13, 11]
[5, 3, 2, 7, 13, 11]
[5, 3, 2, 7, 13, 11]
[5, 3, 2, 7, 13, 11]
[7, 3, 2, 5, 13, 11]
[7, 5, 2, 3, 13, 11]
[7, 5, 3, 2, 13, 11]
[7, 5, 3, 2, 13, 11]
[7, 5, 3, 2, 13, 11]
[7, 5, 3, 2, 13, 11]
[13, 5, 3, 2, 7, 11]
[13, 7, 3, 2, 5, 11]
[13, 7, 5, 2, 3, 11]
[13, 7, 5, 3, 2, 11]
[13, 7, 5, 3, 2, 11]
[13, 7, 5, 3, 2, 11]
[13, 7, 5, 3, 2, 11]
[13, 11, 5, 3, 2, 7]
[13, 11, 7, 3, 2, 5]
[13, 11, 7, 5, 2, 3]
[13, 11, 7, 5, 3, 2]
[13, 11, 7, 5, 3, 2]
```