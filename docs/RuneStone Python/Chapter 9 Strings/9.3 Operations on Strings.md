# 9.3 Operations on Strings

- In general, you cannot perform mathematical operations on strings, even if the strings look like numbers.
- You can use the addition (+) operator, but it serves as a concatenation (smashes 2 strings together), not addition

```python
fruit = "banana"
bakedGood = " nut bread"
print(fruit + bakedGood)

# Output: banana nut bread
```

- The `*`operator also works on strings.  It performs repetition. For example,`'Fun'*3` is `'FunFunFun'`

```python
print("Go" * 6)

name = "Packers"
print(name * 3)

print(name + "Go" * 3)

print((name + "Go") * 3)

'''Output: 
GoGoGoGoGoGo
PackersPackersPackers
PackersGoGoGo
PackersGoPackersGoPackersGo
'''
```