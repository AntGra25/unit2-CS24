# Quiz018

## 1. Solution
```.py
def get_truth() -> str:
    out = "| A | B | C |\n"
    nums = {False: "0", True: "1"}
    a, b, c = False, False, False
    for x in range(1, 9):
        out += f"| {nums[a]} | {nums[b]} | {nums[c]} |\n"
        c = not c
        if x % 2 == 0:
            b = not b
        if x % 4 == 0:
            a = not a
    return out
```
## 2. Proof of Work
![Quiz018](https://github.com/AntGra25/unit2-CS24/assets/142757981/a4bc3c4c-db77-4f01-a7ed-677d81e0b822)

## 3. Truth Table and Circuit
