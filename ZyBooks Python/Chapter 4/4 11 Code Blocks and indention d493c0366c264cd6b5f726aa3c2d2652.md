# 4.11 Code Blocks and indention

- A **code block** is a series of statements that are grouped together
    - The initial code block is not indented
    - A new code block can follow a statement that ends with a colon, such as an "if" or "else"
    - In addition, a new code block must be more indented than the previous code block.
    - **Good practice** is to use the standard recommended 4 columns per indentation level
- A **common error** for new Python programmers is the mixing of tabs and spaces.
    - Use 4 spaces
    - Many editors consider a tab to be equivalent to either 3 or 4 spaces, while **in Python a tab is equivalent only to another tab.**
    - A program that mixes tabs and space to indent code blocks will automatically generate an **IndentationError** from the interpreter in Python 3
    - **Good practice** is to use spaces only when indenting code, and to set text editor options to automatically use spaces when possible.

Example of indentation:

![4%2011%20Code%20Blocks%20and%20indention%20d493c0366c264cd6b5f726aa3c2d2652/Untitled.png](4%2011%20Code%20Blocks%20and%20indention%20d493c0366c264cd6b5f726aa3c2d2652/Untitled.png)

### Special cases

- The number of columns of text considered to be acceptable varies from 80 to 120
- **Good practice** is to use the widely accepted standard of 80 columns.
    - A few exceptions to the rules of indentation deal with very long statements that require more than one line and wrap to the next line.
        - Does not count as a new code block

![4%2011%20Code%20Blocks%20and%20indention%20d493c0366c264cd6b5f726aa3c2d2652/Untitled%201.png](4%2011%20Code%20Blocks%20and%20indention%20d493c0366c264cd6b5f726aa3c2d2652/Untitled%201.png)

![4%2011%20Code%20Blocks%20and%20indention%20d493c0366c264cd6b5f726aa3c2d2652/Untitled%202.png](4%2011%20Code%20Blocks%20and%20indention%20d493c0366c264cd6b5f726aa3c2d2652/Untitled%202.png)