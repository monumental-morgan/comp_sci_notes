# 9.4 Index Operator: Working with the Characters of a String

- I**ndexing operator** (Python uses square brackets to enclose the index) selects a single character from a string.

![Untitled](9%204%20Index%20Operator%20Working%20with%20the%20Characters%20of%20%20704131a9a90a44fba4afe38f26390e7f/Untitled.png)

- This can be used to select specific characters in a string

```python
school = "Luther College"
m = school[2]
print(m)

lastchar = school[-1]
print(lastchar)

'''Output:
t
e
'''
```

- The expression `school[2]`selects the character at index 2 from `school`, and creates a new string containing just this one character. The variable `m`refers to the result.
- **Remember that computer scientists often start counting from zero**
- The expression in brackets is called an **index**