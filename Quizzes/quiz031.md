# Quiz031

## 1. Solution
```.py
from Unit2.unit2_lib import get_sensor, smoothing
from matplotlib import pyplot as plt

sensor1 = get_sensor()
sensor2 = get_sensor(id=2)
sm = []
avg = []
t = []
for i in range(len(sensor1)):
    sm.append(sensor1[i] + sensor2[i])
    avg.append((sensor1[i] + sensor2[i]) / 2)
    t.append(i)
ys, xs = smoothing(x=sm)
ya, xa = smoothing(x=avg)


plt.style.use('ggplot')
plt.subplot(2, 1, 1)
plt.plot(sensor1)
plt.title('Sensor 1')
plt.subplot(2, 1, 2)
plt.plot(sensor2)
plt.title('Sensor 2')
plt.subplots_adjust(hspace=0.5)
plt.show()

plt.subplot(2, 1, 1)
plt.plot(ys, xs)
plt.title('Sum')
plt.subplot(2, 1, 2)
plt.plot(ya, xa)
plt.title('Average')
plt.subplots_adjust(hspace=0.5)
plt.show()
```
## 2. Proof of Work

## 3. 
