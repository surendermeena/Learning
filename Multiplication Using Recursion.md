def multiplication(m,n):
    if n ==0:
        return 0
    small_out = multiplication(m,n-1)
    output = (small_out) + m
    return output
    
from sys import setrecursionlimit
setrecursionlimit(10**6)

m = int(input())
n = int(input())
product = multiplication(m,n)
print(product)
