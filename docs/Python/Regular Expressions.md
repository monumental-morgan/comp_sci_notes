# Regular Expressions

## [Official Documentation](https://docs.python.org/3.8/library/re.html#)

![Untitled](regular-expressions.png)

### **[Remove Numbers from String](https://www.studytonight.com/python-howtos/remove-numbers-from-string-in-python)**

```python
#regex module
import re

#original string
string1 = "Hello!James12,India2020"

pattern = r'[0-9]'

# Match all digits in the string and replace them with an empty string
new_string = re.sub(pattern, '', string1)

print(new_string)

'''Output
Hello!James,India
'''
```

### Useful Examples of Splitting

```python
# Python3 code to demonstrate working of
# Add space between Numbers and Alphabets in String
# using regex + sub()
import re
 
# initializing string
test_str = 'geeks4geeks is1for10geeks'
 
# printing original String
print("The original string is : " + str(test_str))
 
# using sub() to solve the problem
res = re.sub('(\d+(\.\d+)?)', r' \1 ', test_str)
 
# printing result
print("The space added string : " + str(res))

'''Ouput

The original string is : geeks4geeks is1for10geeks
The space added string : geeks 4 geeks is 1 for 10 geeks
'''
```

```python
# Python3 code to demonstrate working of
# Splitting text and number in string
# Using re.compile() + re.match() + re.groups()
import re
 
# initializing string
test_str = "Geeks4321"
 
# printing original string
print("The original string is : " + str(test_str))
 
# Using re.compile() + re.match() + re.groups()
# Splitting text and number in string
temp = re.compile("([a-zA-Z]+)([0-9]+)")
res = temp.match(test_str).groups()
 
# printing result
print("The tuple after the split of string and number : " + str(res))

'''Output
The original string is : Geeks4321
The tuple after the split of string and number : ('Geeks', '4321')
'''
```

Cheat Sheet