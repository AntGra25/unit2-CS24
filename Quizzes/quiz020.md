# Quiz020

## 1. Solution
```.py
import random
random.seed(1234)

def produce(n:int, m:int, s:int) -> str:
    out = f"|{'x'.center(10)}|{'y(x)'.center(10)}|\n"
    for i in range(n):
        x = random.randint(0, 100)
        y = f"{x**(0.5*((m/s)**2)):.2f}"
        out += f"|{str(x).center(10)}|{y.center(10)}|\n"
    return out
```
## 2. Proof of Work
![Quiz020](https://github.com/AntGra25/unit2-CS24/assets/142757981/e8f51c02-302e-43e6-98aa-9c5717a3323f)

## 3. Proof
![Quiz020C](https://github.com/AntGra25/unit2-CS24/assets/142757981/20c317a5-6141-4e57-a97d-b7932aa286e1)
