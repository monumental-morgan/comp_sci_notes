# 3.1 String Basics

# Strings and string literals

- A **string** is a sequence of characters, like the text MARY, that can be stored in a variable.
- A **string literal** is a string value specified in the source code of a program.
- The **len()** built-in function can be used to find the length of a string (and any other sequence type).
- .split() will break the string into a list
- end=' ' will stop print() from creating a newline
    - print('Continue bidding?', end=' ')

![3%201%20String%20Basics%20ec69126238df4f41a72b1f3d1246bcaa/Untitled.png](3%201%20String%20Basics%20ec69126238df4f41a72b1f3d1246bcaa/Untitled.png)

- As a sequence type, every character in a string has an index, or position, starting at 0 from the leftmost character.
    - A programmer can access a character at a specific index by appending **brackets [ ]** containing the index:
    
    ![3%201%20String%20Basics%20ec69126238df4f41a72b1f3d1246bcaa/Untitled%201.png](3%201%20String%20Basics%20ec69126238df4f41a72b1f3d1246bcaa/Untitled%201.png)
    
    - Negative numbers will make it start from the right side rather than left

# Changing String variables and concatenating strings

- Individual characters of a string cannot be changed, but the string itself can be altered by updating the entire variable.
- Concatenation: combining strings
    
    ![3%201%20String%20Basics%20ec69126238df4f41a72b1f3d1246bcaa/Untitled%202.png](3%201%20String%20Basics%20ec69126238df4f41a72b1f3d1246bcaa/Untitled%202.png)