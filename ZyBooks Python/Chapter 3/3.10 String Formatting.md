# 3.10 String Formatting

![3%2010%20String%20Formatting%2033d71cc6bb354208b53ca5328ceb1b60/Untitled.png](3%2010%20String%20Formatting%2033d71cc6bb354208b53ca5328ceb1b60/Untitled.png)

![3%2010%20String%20Formatting%2033d71cc6bb354208b53ca5328ceb1b60/Untitled%201.png](3%2010%20String%20Formatting%2033d71cc6bb354208b53ca5328ceb1b60/Untitled%201.png)

## Format Specification

- A format specification inside of a replacement field allows a value's formatting in the string to be customized
    - a variable with the integer value 4 can be output as a floating-point number (4.0) or with leading zeros (004).

![3%2010%20String%20Formatting%2033d71cc6bb354208b53ca5328ceb1b60/Untitled%202.png](3%2010%20String%20Formatting%2033d71cc6bb354208b53ca5328ceb1b60/Untitled%202.png)

## Referencing format() values correctly

- The colon : in the replacement field separates the "what" on the left from the "how" on the right.
    - side may be omitted (inferred positional replacement)
    - a number (positional replacement)
    - a name (named replacement)

![3%2010%20String%20Formatting%2033d71cc6bb354208b53ca5328ceb1b60/Untitled%203.png](3%2010%20String%20Formatting%2033d71cc6bb354208b53ca5328ceb1b60/Untitled%203.png)

## Alternative string formatting

- A formatted string literal or f-string is a string literal that is prefixed with 'f' or 'F'. These strings may contain replacement fields, which are expressions delimited by curly braces {}. While other string literals always have a constant value, formatted strings are really expressions evaluated at run time.
- print(f'Amount: ${dollars:.2f}')
    
    Ex: Amount: $1.25