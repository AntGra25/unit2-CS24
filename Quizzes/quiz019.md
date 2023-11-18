# Quiz019

## 1. Solution
```.py
def get_truth2() -> str:
    out = "| A | B | C | AB + not B + not CB |\n"
    nums = {False: "0", True: "1"}
    a, b, c = False, False, False
    for x in range(1, 9):
        out += f"| {nums[a]} | {nums[b]} | {nums[c]} | {nums[a and b or not b or not c and b].center(19)} |\n"
        c = not c
        if x % 2 == 0:
            b = not b
        if x % 4 == 0:
            a = not a
    return out


print(get_truth2())

```
## 2. Proof of Work
![Quiz019](https://github.com/AntGra25/unit2-CS24/assets/142757981/4a9c375b-0d81-45b5-9877-367ff6cae121)
