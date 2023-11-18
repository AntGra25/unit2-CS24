# Quiz023

## 1. Solution
```.py
from matplotlib import pyplot as plt

def absplot():
    x_out = []
    y_out = []
    x = -10
    for i in range(100):
        y = abs(x)
        x_out.append(x)
        y_out.append(y)
        x += 0.2
    return x_out, y_out

x, y = absplot()
plt.style.use('ggplot')
plt.plot(x, y, color='r')
plt.xlabel("x", fontsize=20)
plt.ylabel("$f(x) = |x|$", fontsize=20)
plt.show()

```
## 2. Proof of Work
![Quiz023](https://github.com/AntGra25/unit2-CS24/assets/142757981/15d14fc1-d7ff-4771-87a0-94a0a494b191)

## 3. Convert to Decimal
![Quiz023C](https://github.com/AntGra25/unit2-CS24/assets/142757981/ca987acd-b0d5-4d62-9a5c-afbe522eb916)
