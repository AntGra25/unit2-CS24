# Quiz017

## 1. Solution
```.py
def get_l3tt3r(msg: str) -> str:
    out = ""
    code = {"a": "4", "e": "3", "i": "1", "o": "0", " ": "_"}
    for let in msg:
        if let.lower() in code:
            out += code[let.lower()]
        else:
            out += let
    return out
```
## 2. Proof of Work
![Quiz017](https://github.com/AntGra25/unit2-CS24/assets/142757981/210fd135-2140-4a78-8f7f-102c26f433d5)

## 3. Boolean Circuit
![Quiz017C](https://github.com/AntGra25/unit2-CS24/assets/142757981/9d564842-9e7e-4557-842c-9a66f9525a13)
