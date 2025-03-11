# Miryusif-Abdullayev
Lab 3
import math

epsilon = 0.01
x = 0.5

term = math.sin(x)
P = term
n = 1

while abs(term) >= epsilon:
    term *= -math.sin(x) / (n + 1)
    P += term
    n += 1

print(P)
