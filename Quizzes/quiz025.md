# Quiz025

## 1. Solution
```.py
import numpy as np
from matplotlib import pyplot as plt

sensorA = [16, 24, 24, 9, 23, 26, 26, 23, 25, 14]
sensorB = [2, 19, 25, 10, 11, 24, 17, 7, 24, 17]
sensorC = [15, 11, 24, 21, 6, 2, 18, 27, 1, 16]

time = []
mean = []
std = []
minimum = []
maximum = []
for i in range(len(sensorA)):
    mean.append((sensorA[i] + sensorB[i] + sensorC[i]) / 3)
    std.append(np.std([sensorA[i], sensorB[i], sensorC[i]]))
    minimum.append(min([sensorA[i], sensorB[i], sensorC[i]]))
    maximum.append(max([sensorA[i], sensorB[i], sensorC[i]]))
    time.append(i)

plt.style.use('ggplot')
plt.fill_between(time, maximum, minimum, alpha=0.5, color='gray', label='Maximum & Minimum Values')
plt.errorbar(time, mean, std, fmt="+", label='Standard Deviation', color='blue')
plt.ylim(0, 35)
plt.legend()
plt.show()

```
## 2. Proof of Work
![Quiz025](https://github.com/AntGra25/unit2-CS24/assets/142757981/013d84e3-abbc-492a-96cd-372e7ec8cb5a)


## 3. RGB to Hex Color
![Quiz025C](https://github.com/AntGra25/unit2-CS24/assets/142757981/bfa738ff-a334-48ab-ae83-ad75b4dd96d2)
