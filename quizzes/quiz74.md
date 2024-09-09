```

str  = '1011101110' 
prity_bit = ' ' // 1 or 0 
count_0 = 0 
count_1 = 0 
loop in range(length(str)): 
  if i == 0 
    prity_bit = str[i]
  if str[i] == '0'
    count_0 += 1 
  if str[i] == '1'
    count_1 +=1 
  if count_1%2 ==0 and prity_bit == 1: 
    return: 'error free' 
  if count_0%2 == 0 and prity_bit == 0:
    return: "error free" 
  else: 
    return: "error detected"
```
