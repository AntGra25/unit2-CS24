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

## 3. 
