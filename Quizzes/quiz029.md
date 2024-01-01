# Quiz029

## 1. Solution
```.py
def sort_dict(in_dict: dict) -> dict:
    out_dict = {}
    x = list(in_dict.values())
    k = list(in_dict.keys())
    for i in range(len(x)):
        for n in range(i + 1, len(x)):
            if type(x[i]) == str and type(x[n]) == int:
                x[i], x[n] = x[n], x[i]
                k[i], k[n] = k[n], k[i]
            elif type(x[i]) == int and type(x[n]) == int and x[i] > x[n]:
                x[i], x[n] = x[n], x[i]
                k[i], k[n] = k[n], k[i]
            elif type(x[i]) == str and type(x[n]) == str and ascii(k[i]) > ascii(k[n]):
                x[i], x[n] = x[n], x[i]
                k[i], k[n] = k[n], k[i]
    for i in range(len(x)):
        out_dict[k[i]] = x[i]

    return out_dict
```
## 2. Proof of Work
![Quiz029](https://github.com/AntGra25/unit2-CS24/assets/142757981/3e7da7dd-1201-4aa7-88ca-adb094e6f41c)

## 3. Graph of y = sin(2*pi*x) for 0 < x < 1

```.py
from matplotlib import pyplot as plt
import math

x = []
y = []

for i in range(101):
    num = i/100
    x.append(num)
    y.append(math.sin(math.pi * 2 * num))

plt.style.use('ggplot')
plt.plot(x, y)
plt.show()
```

![Quiz029 1](https://github.com/AntGra25/unit2-CS24/assets/142757981/644f9ebe-677e-415a-949a-bdab5c8636e5)
