# 9.5 String Methods & String Format

- “dot notation” is the way we connect the name of an object to the name of a method it can perform.

```python
ss = "Hello, World"
print(ss.upper())

tt = ss.lower()
print(tt)

'''Output:
HELLO, WORLD
hello, world
'''
```

- In addition to `upper`and `lower`, the following table provides a summary of some other useful string methods.

![Untitled](9%205%20String%20Methods%20&%20String%20Format%200b4d8e1d4b23449daffe90ce05759e10/Untitled.png)

```python
ss = "    Hello, World    "

els = ss.count("l")
print(els)

print("***" + ss.strip() + "***")
print("***" + ss.lstrip() + "***")
print("***" + ss.rstrip() + "***")

news = ss.replace("o", "***")
print(news)

'''Output:
3
***Hello, World***
***Hello, World    ***
***    Hello, World***
    Hell***, W***rld
'''
```

# Zach’s Notes

- What I used to get all strings the same length (this was useful for adding numbers at the end and keeping them in line (SEE UNIT 5 ASSIGNMENT table_3 function for more info)

```python
if len(m) <= 26:
	m += ' '
```

# 9.5.1 String Format Method

### What Zach Uses

- Abbreviated `format` in front of string and variable referenced in curly brackets.

```python
a = 'world'
print(f"hello {a}")
```

- See **[Python 3's f-Strings: An Improved String Formatting Syntax (Guide)](https://realpython.com/python-f-strings/)**

### Textbook

- The string method `format`,  makes substitutions into places in a string enclosed in braces.

```python
person = input('Your name: ')
greeting = 'Hello {}!'.format(person)
print(greeting)
```

- There can be multiple substitutions, with data of any type. Next we use floats. Try original price $2.50 with a 7% discount:

```python
origPrice = float(input('Enter the original price: $'))
discount = float(input('Enter discount percentage: '))
newPrice = (1 - discount/100)*origPrice
calculation = '${} discounted by {}% is ${}.'.format(origPrice, discount, newPrice)
print(calculation)

'''Output:
$5.10 discounted by 6.1% is $4.7889.
'''
```

- The parameters are inserted into the braces in order.
- Format strings can give further information inside the braces showing how to specially format data.
- For two decimal places, put `:.2f`inside the braces for the monetary values:

```python
origPrice = float(input('Enter the original price: $'))
discount = float(input('Enter discount percentage: '))
newPrice = (1 - discount/100)*origPrice
calculation = '${:.2f} discounted by {}% is ${:.2f}.'.format(origPrice, discount, newPrice)
print(calculation)

'''Output
$5.10 discounted by 6.1% is $4.79.
'''
```

- The 2 in the format modifier can be replaced by another integer to round to that specified number of digits.

**Note: If you need curly braces in the string itself, use double {{**

```python
letter = """
Dear {0} {2}.
 {0}, I have an interesting money-making proposition for you!
 If you deposit $10 million into my bank account, I can
 double your money ...
"""

print(letter.format("Paris", "Whitney", "Hilton"))
print(letter.format("Bill", "Henry", "Gates"))

'''Output:
Dear Paris Hilton.
 Paris, I have an interesting money-making proposition for you!
 If you deposit $10 million into my bank account, I can
 double your money ...

Dear Bill Gates.
 Bill, I have an interesting money-making proposition for you!
 If you deposit $10 million into my bank account, I can
 double your money ...
'''
```