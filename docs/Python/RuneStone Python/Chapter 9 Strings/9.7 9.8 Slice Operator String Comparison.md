# 9.7/8 Slice Operator/String Comparison

- A substring of a string is called a **slice**
- Selecting a slice is similar to selecting a character
- 

```python
singers = "Peter, Paul, and Mary"
print(singers[0:5])
print(singers[7:11])
print(singers[17:21])

'''
singers = "Peter, Paul, and Mary"
print(singers[0:5])
print(singers[7:11])
print(singers[17:21])

Output:

Peter
Paul
Mary
'''
```

- The slice operator `[n:m]`returns the part of the string from the n’th character to the m’th character, including the first but excluding the last.
    - Similar to range function

# 9.8 String Comparison

- Using boolean to compare strings

```python
word = "banana"
if word == "banana":
    print("Yes, we have bananas!")
else:
    print("Yes, we have NO bananas!")

''' Output
Yes, we have bananas!
'''
```