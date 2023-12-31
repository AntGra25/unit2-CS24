# Quiz021

## 1. Solution
```.py
import matplotlib.pyplot as plt
import random
random.seed(1234)
def produce(n: int, m: int, s: int):
    x_out = []
    y_out = []
    for _ in range(n):
        x = random.randint(0,100)
        y = x ** (0.5 * ((m/s)**2))
        x_out.append(x)
        y_out.append(y)
    return y_out, x_out


plt.style.use('ggplot')
y, x = produce(n=10, m=5, s=2)

plt.plot(x, y, color='r', marker="o")
plt.xlabel("x", fontsize=20)
plt.ylabel("$y=x^{(1/2)(m/s)}$", fontsize=20)
plt.show()
```
## 2. Proof of Work
![Quiz021](https://github.com/AntGra25/unit2-CS24/assets/142757981/c733413d-9536-47f4-ad9f-2c2241955b8a)

## 3. Truth Table
![Quiz021C](https://github.com/AntGra25/unit2-CS24/assets/142757981/c3e3ae2f-0c78-48e5-84c0-ac7e02068bdf)
