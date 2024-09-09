```
size = length(data)/3
first = " "
for i in range(size):
  first += data[i]
second = " "
for i in range(size, size *2):
  second += data[i]
third = " "
for i in range(size*2, size *3):
  third += data[i]
if (first == second) AND (second == third):
  print(True)
else:
  print(False)
```
