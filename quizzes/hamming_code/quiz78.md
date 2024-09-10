Create a function get_message that creates the template for the final message with -1 in the positions of the parity bits 

```
msg = '1011'
n = length(msg)
def get_k(n):
  k = 0
  while 2 **k < k+n+1
    K+=1
  end while
  return K

def get_pos(k):
  pos_list = []
  for i in length(k)
    pos = 2** i-1
    pos_list.append(pos)
  return pos_list

def get_msg(msg):
  n = length(msg)
  k = get_k(n)
  pos_list = get_pos(k)
  msg_temp= []

msg_index = 0

for i in range(n+k):
  if i in pos_list:
    msg_temp.append(-1)
  else:
    msg_tamp.append(integer(msg[msg_index]))
    msg_index += 1 
  
```

