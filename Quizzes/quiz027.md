# Quiz027

## 1. Solution
```.py
def count_letters(my_dict: dict, msg: str) -> dict:
    for letter in msg:
        if letter in my_dict:
            my_dict[letter] += 1
    return my_dict
```
## 2. Proof of Work
![Quiz027](https://github.com/AntGra25/unit2-CS24/assets/142757981/16e30754-57a7-41f0-81d0-b4b503daef3a)

## 3. Colors in a 6 bit Computer

2<sup>6</sup> = 64 colors
