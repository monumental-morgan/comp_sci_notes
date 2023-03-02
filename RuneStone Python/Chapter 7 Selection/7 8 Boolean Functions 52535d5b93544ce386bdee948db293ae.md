# 7.8 Boolean Functions

# Example of Outputting Boolean Values

```python
def isDivisible(x, y):
    if x % y == 0:
        result = True
    else:
        result = False

    return result

print(isDivisible(10, 5))
```