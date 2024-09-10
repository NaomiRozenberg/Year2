```py
def get_k(n):
    k = 0
    while 2 ** k < k + n + 1:
        k += 1
    return k


def get_pos(k):
    pos_list = []
    for i in range(k):
        pos = 2 ** i - 1
        pos_list.append(pos)
    return pos_list


def get_equation(n_k, p):
    result_list = []
    for i in range(n_k):
        if i & (1 << (p - 1)) != 0:
            result_list.append(i)
    return result_list

def get_msg(msg):
    n = len(msg)
    k = get_k(n)
    pos_list = get_pos(k)
    msg_temp = []
    msg_index = 0

    for i in range(n + k):
        if i in pos_list:
            msg_temp.append(-1)
        else:
            msg_temp.append(int(msg[msg_index]))
            msg_index += 1

    for p in range(1, k + 1):
        numbers = get_equation(len(msg_temp), p)
        parity_value = 0
        for index in numbers:
            if msg_temp[index] != -1:
                parity_value ^= msg_temp[index]
        msg_temp[2 ** (p - 1) - 1] = parity_value

    return msg_temp

msg1 = '1011'
ham_msg1 = get_msg(msg1)
print(ham_msg1)
msg2 = '1111'
ham_msg2 = get_msg(msg2)
print(ham_msg2)
msg3 = '1111'
ham_msg3 = get_msg(msg3)
print(ham_msg3)

```
<img width="1359" alt="Screenshot 2024-09-10 at 11 33 30" src="https://github.com/user-attachments/assets/519e48ca-caf9-4999-b147-eb34eb3b9b8b">
