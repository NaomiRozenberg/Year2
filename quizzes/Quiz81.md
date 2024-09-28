81. Trace the following program for the input N= ‘AB’


```
def PERM(s:str, k:int):
    if k == len(s):
        return [s]
    else:
        out = []
        for i in range(len(s)):
            t = swap_letter(s, k, i)
            out.extend(permute(t,k+1))

        return out
```
