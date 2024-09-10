Create a function get_equation that produces the numbers associated with the parity bit provided. Remember that the pattern is: “the first parity 1 includes the numbers that have 1 in the first bit when written in binary”

```
def get_equation(n+k, p):
    result_list = []
    for i in range(n+k):
        if i & (1 << (p - 1)) != 0:
            result_list.append(i)
    return result_list
```
