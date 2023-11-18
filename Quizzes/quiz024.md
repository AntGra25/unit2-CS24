# Quiz024

## 1. Solution
```.py
import matplotlib.pyplot as plt
import numpy as np

plt.style.use('ggplot')
h = [57.0, 56.0, 57.0, 56.0, 55.0, 54.0, 54.0, 54.0, 53.0, 53.0, 54.0, 53.0, 53.0, 52.0, 52.0, 51.0, 51.0, 51.0, 50.0,
     50.0, 49.0, 50.0, 49.0, 49.0, 48.0, 49.0, 49.0, 48.0, 48.0, 48.0, 49.0]  # 32 values every 10 min
time = []
t = 0
for i in range(len(h)):
    time.append(t)
    t += 10  # 10min

plt.scatter(time, h, color="blue")
plt.xlabel("Time (min)")
plt.ylabel("Humidity (%)")

m, b = np.polyfit(time, h, 1)
plt.title(f"Linear model h(t) = {m:.2f}t+{b:.2f}")

time_model = []
h_model = []
t = 0
for i in range(len(h)):
    time_model.append(t)
    h_model.append(m*t + b)
    t += 10

plt.plot(time_model, h_model, color='black')
plt.show()

```
## 2. Proof of Work
![Quiz024](https://github.com/AntGra25/unit2-CS24/assets/142757981/c3b53211-2ce5-4075-87f3-b3e260bb1fd6)

## 3. Convert to RGB
![Quiz024C](https://github.com/AntGra25/unit2-CS24/assets/142757981/0778d784-eba6-4298-9bd9-42b29efe771d)

