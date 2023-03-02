# 2.10 Representing Text

# Unicode

- Python uses **Unicode** to represent every possible character as a unique number, known as a **code point**
    - Ex: The character 'G' has the code point decimal value of 71

![2%2010%20Representing%20Text%20dc3a0e3bdd494dfba6b89cf8b3a495e8/Untitled.png](2%2010%20Representing%20Text%20dc3a0e3bdd494dfba6b89cf8b3a495e8/Untitled.png)

# Escape Sequences

- **\** is a term that the interpreter recognizes as the start to a special character, like **\n** for **newline**.
- These two character sequences are escape sequences

![2%2010%20Representing%20Text%20dc3a0e3bdd494dfba6b89cf8b3a495e8/Untitled%201.png](2%2010%20Representing%20Text%20dc3a0e3bdd494dfba6b89cf8b3a495e8/Untitled%201.png)

## Raw strings and converting text

- Escape sequences can be ignored using a **raw string**
    - A raw string is created by adding an 'r' before a string literal, as in **r'this is a raw string\''**, which would output as **this is a raw string\'**

![2%2010%20Representing%20Text%20dc3a0e3bdd494dfba6b89cf8b3a495e8/Untitled%202.png](2%2010%20Representing%20Text%20dc3a0e3bdd494dfba6b89cf8b3a495e8/Untitled%202.png)

- **ord()** returns the encoded integer value for the first character of a string
    - **chr()** does the reverse, gives the character for the encoded integer given

## Formatting text