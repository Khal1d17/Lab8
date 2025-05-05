import math

a = 0.000001  
eps = 1e-6   

while (b - a) > eps:
    c = (a + b) / 2
    fa = a + math.log(a) - 0.5
    fc = c + math.log(c) - 0.5

    if fa * fc < 0:
        b = c
    else:
        a = c

root = (a + b) / 2
print("Təqribi kök:", root)
