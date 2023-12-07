# Quiz032

## 1. Solution
```.py
from Unit2.unit2_lib import get_sensor
from matplotlib import pyplot as plt
from matplotlib.gridspec import GridSpec

plt.style.use('ggplot')
s4 = get_sensor(id=4)
s5 = get_sensor(id=5)

difference = []
for i in range(len(s4)):
    difference.append(-s4[i] - s5[i])

fig = plt.figure(figsize=(10, 5))
grid = GridSpec(3, 4, figure=fig)
plt.subplots_adjust(hspace=0.5)

box1 = fig.add_subplot(grid[0:3, 1:3])
plt.plot(difference, color='red')
plt.title('-Sensor#4 - Sensor#5')

box2 = fig.add_subplot(grid[1, 0])
plt.plot(s4, color='black')
plt.title('Sensor id=4')
plt.ylim([0, 100])
plt.xlim([0, 800])

box3 = fig.add_subplot(grid[1, 3])
plt.plot(s5, color='black')
plt.title('Sensor id=5')
plt.ylim([0, 100])
plt.xlim([0, 800])

plt.show()
```
## 2. Proof of Work

## 3. 
