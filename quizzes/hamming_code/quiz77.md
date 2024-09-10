Create a function get_equation that produces the numbers associated with the parity bit provided. Remember that the pattern is: “the first parity 1 includes the numbers that have 1 in the first bit when written in binary”

```
def get_indices(n+k, p):
   result_list = []

    For i from 0 to n+k - 1:
        If i AND (1 << (p - 1)) is not 0:
            Add i to result_list

    Return result_list

```
