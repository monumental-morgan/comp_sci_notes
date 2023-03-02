# 6.2/3 Function Return Values & Unit Testing

- Most functions require arguments, values that control how the function does its job

### Fruitful Functions

- Functions that return values

### Non-Fruitful Functions

- Function that doesn’t return value
- Known as a **procedure** in other programming languages

# 6.3 Unit Testing

- a test asserts something about the state of the program at a particular point in its execution.
- **unit test** is an automatic procedure used to validate that individual units of code are working properly
- One way to implement unit tests in Python is with `assert`
    - Following the word assert there will be a python expression.
    - If that expression evaluates to the Boolean `False`, then the interpreter will raise a runtime error.
    - If the expression evaluates to `True`, then nothing happens and the execution goes on to the next line of code.

Ex:

```python
assert type(9//5) == int
assert type(9.0//5) == int
```

- First line will pass, second line will fail, cause it is a float not an int
- We can add `assert`statements that will cause an error to be flagged sooner rather than later, which might make it a lot easier to debug

### `assert` with `for` loops

Ex:

```python
lst = ['a', 'b', 'c']
first_type = type(lst[0])
for item in lst:
    assert type(item) == first_type

lst2 = ['a', 'b', 'c', 17]
first_type = type(lst2[0])
for item in lst2:
    assert type(item) == first_type
```

- 1st assert passes, but 2nd assert fails because there is a different type in the list

### Return Value Test

- Testing whether a function returns the correct value is the easiest test case to define

Ex:

```python
def square(x):
#raise x to the second power
    return x*x
print('testing square function')
assert square(3) == 9
```

### [unittest Module](https://www.youtube.com/watch?v=6tNS--WetLI)

- In larger projects, other testing harnesses are used instead of `assert`, such as the python`unittest`module.
    - Those provide some output summarizing tests that have passed as well as those that failed.
- Have a second .py file that will be a module
    - named test_whatever.py