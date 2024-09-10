```
obj0 = 0
obj1 = 0
obj2 = 0
obj3 = 0
IP = [obj0, obj1, obj2,obj3]

While obj0<= 255:
  print(IP)
  obj3 +=1

  if obj3 == 256:
    obj3 = 0
    obj2 +=1

  if obj2 == 256:
    obj2 = 0
    obj1 +=1

  if obj1 == 256:
    obj1 = 0
    obj0 +=1 

end while 
  

```
