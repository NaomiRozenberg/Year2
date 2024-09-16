80. Trace the following program for the input N=[4,5,8,7]


def FUNC(N):
    if len(N) == 1:
        return N[0]
    
    M = FUNC(N[1:])
    
    if N[0] > M:
        return N[0]
    else:
        return M
![Uploading IMG_0664.jpg…]()
