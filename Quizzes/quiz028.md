# Quiz028

## 1. Solution
```.py
def invert(in_dict: dict):
    out_dict = {}
    keys = list(in_dict.keys())
    values = list(in_dict.values())
    for i in range(len(in_dict)):
        if values[i] not in out_dict:
            out_dict[values[i]] = []
        out_dict[values[i]].append(keys[i])
    return out_dict
```
## 2. Proof of Work
![Quiz028](https://github.com/AntGra25/unit2-CS24/assets/142757981/96dbea00-bc7e-40d1-8faa-014e19a7414e)


## 3. Binary 1011 + 1101
![Quiz028C](https://github.com/AntGra25/unit2-CS24/assets/142757981/3ffa7939-daac-4975-84d3-e02005e0dbe9)

