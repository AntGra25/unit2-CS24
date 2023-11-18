# Quiz022

## 1. Solution
```.py
from matplotlib import pyplot as plt

def prblplot():
    x_out = []
    y_out = []
    x = -10
    for i in range(100):
        y = 2*(x + 5)**2
        x_out.append(x)
        y_out.append(y)
        x += 0.2
    return x_out, y_out

x, y = prblplot()
plt.style.use('ggplot')
plt.plot(x, y, color='r')
plt.xlabel("x", fontsize=20)
plt.ylabel("$y=2(x + 5)^{2}$", fontsize=20)
plt.show()
```
## 2. Proof of Work
![Quiz022](https://github.com/AntGra25/unit2-CS24/assets/142757981/24e9f3e7-2ba1-4a43-8270-2efabfeaa6d6)

## 3. Circuit
![Quiz022C](https://github.com/AntGra25/unit2-CS24/assets/142757981/d107f7db-c746-4eb7-b25c-72b107474e84)
