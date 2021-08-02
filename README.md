# collatz_conjecture
import matplotlib.pyplot as plt
import numpy as np

def collatz(x):
    sequence = [x]
    while x != 1:
        if x % 2 == 0:
            x = x/2
        else:
            x = 3*x +1
        sequence.append(x)
    return sequence
    
x = 257
plt.plot(collatz(x));

